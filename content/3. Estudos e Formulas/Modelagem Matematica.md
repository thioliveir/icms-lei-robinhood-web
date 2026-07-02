---
title: Modelagem Matemática do ICMS Robin Hood
tags:
  - formulas
  - modelagem-matematica
  - economia
  - estatistica
date: 2026-07-01
---

# 🧮 Modelagem Matemática do ICMS Robin Hood (Minas Gerais)

Esta nota consolida a modelagem matemática utilizada para calcular a cota-parte de ICMS de cada um dos 853 municípios de Minas Gerais, com base na Lei nº 18.030/2009 (atualizada pela Lei nº 24.431/2023).

---

## 🏛️ A Equação Geral do Repasse ($IP_{\text{total}}$)

O Índice de Participação total de um município $i$ no repasse do ICMS ($IP_{\text{total}, i}$) é a soma ponderada de sua participação em cada um dos critérios definidos no Art. 1º da Lei. A soma de todos os índices de participação de todos os municípios do estado resulta em $100\%$ (ou $1,0$):

$$\sum_{i=1}^{853} IP_{\text{total}, i} = 100\%$$

A equação geral para o município $i$ é expressa por:

$$IP_{\text{total}, i} = \sum_{k=1}^{18} (IP_{k, i})$$

Onde cada parcela representa o índice individual do município no critério $k$ ponderado pelo peso percentual atribuído pela lei.

---

## 📊 Pesos e Fórmulas dos Critérios Ativos

A tabela abaixo agrupa os critérios por categoria temática, facilitando a análise de impacto:

| Categoria | Critério ($k$) | Peso (%) | Equação Base / Componentes | Nota de Estudo |
| :--- | :--- | :--- | :--- | :--- |
| **Econômica** | $IP_{1, i}$ (VAF) | $75,00\%$ | $\frac{VAF_i}{\sum VAF} \times 75\%$ | [[VAF\|VAF]] |
| **Territorial** | $IP_{2, i}$ (Área Geográfica) | $1,00\%$ | $\frac{\text{Área}_i}{\sum \text{Área}} \times 1\%$ | [[Area Geografica\|Área Geográfica]] |
| **Demográfica** | $IP_{4, i}$ (50 Mais Populosos) | $2,00\%$ | $\frac{\text{Pop}_i}{\sum_{50} \text{Pop}} \times 2\%$ *(se na lista)* | [[50 Municipios Mais Populosos\|50 Populosos]] |
| **Desenvolvimento Social** | $IP_{5, i}$ (Educação) | $10,00\%$ | $\frac{IQE_i}{\sum IQE} \times 10\%$ | [[Educacao\|Educação]] |
| | $IP_{15, i}$ (Esportes) | $0,50\%$ | $\frac{\text{Atividades Ponderadas}_i}{\sum \text{Atividades Ponderadas}} \times 0,5\%$ | [[Esportes\|Esportes]] |
| **Socioambiental** | $IP_{8, i}$ (Meio Ambiente) | $1,10\%$ | $(P_{\text{san}} \times 0,4545) + (P_{\text{cons}} \times 0,4545) + (P_{\text{mata}} \times 0,091)$ | [[Meio Ambiente\|Meio Ambiente]] |
| **Desenvolvimento Local** | $IP_{6, i}$ (Produção Alimentos) | $1,00\%$ | $(F_1 \times 0,35) + (F_2 \times 0,30) + (F_3 \times 0,30) + (F_4 \times 0,05)$ | [[Producao de Alimentos\|Alimentos]] |
| | $IP_{16, i}$ (Turismo) | $0,50\%$ | $\frac{\text{Investimento Ponderado}_i}{\sum \text{Investimento Ponderado}} \times 0,5\%$ | [[Turismo\|Turismo]] |
| **Compensatória** | $IP_{12, i}$ (Mineradores) | $0,01\%$ | $\text{Proporção Fixa IUM de 1988} \times 0,01\%$ | [[Municipios Mineradores\|Mineradores]] |
| | $IP_{13, i}$ (Recursos Hídricos) | $0,25\%$ | $\frac{\text{Base Alagamento}_i}{\sum \text{Base Alagamento}} \times 0,25\%$ | [[Recursos Hidricos\|Recursos Hídricos]] |
| | $IP_{14, i}$ (Sedes Prisionais) | $0,50\%$ | $\frac{\text{Pop Carcerária}_i}{\sum \text{Pop Carcerária}} \times 0,5\%$ | [[Sedes de Penitenciarias\|Presídios]] |
| **Redistributiva** | $IP_{11, i}$ (Cota Mínima) | $1,50\%$ | $\frac{1,50\%}{853} \approx 0,0017585\%$ (Igual para todos) | [[Cota Minima\|Cota Mínima]] |
| | $IP_{17, i}$ (ICMS Solidário) | $1,89\%$ | $\frac{\text{Pop}_i}{\sum_{\text{Elegíveis}} \text{Pop}} \times 1,89\%$ | [[ICMS Solidario\|ICMS Solidário]] |
| | $IP_{18, i}$ (Mínimo Per Capita) | $3,75\%$ | $\frac{\text{Complemento}_i}{\sum \text{Complemento}} \times 3,75\%$ | [[Minimo Per Capita\|Mínimo Per Capita]] |

*Nota: Critérios III (População), IX (Saúde) e X (Receita Própria) possuem peso de $0,00\%$ pois foram revogados.*

---

## 📈 Análise Matemática dos Subcomponentes Principais

### 1. O Submodelo da Educação ($IQE_i$)
O Índice de Qualidade da Educação ($IQE_i$), que rege os $10\%$ do repasse de educação, é modelado de forma a ponderar eficiência e equidade:

$$IQE_i = 0,50 \cdot IRAP_i + 0,20 \cdot IRE_i + 0,15 \cdot IAE_i + 0,15 \cdot IGE_i$$

Este submodelo representa uma combinação linear de quatro dimensões de desempenho escolar ($IRAP$), rendimento ($IRE$), atendimento ($IAE$) e gestão ($IGE$), fornecendo incentivos financeiros expressivos para melhorias pedagógicas reais.

### 2. O Submodelo Ecológico ($IP_{MA, i}$)
O repasse de Meio Ambiente ($1,10\%$) é estruturado em três variáveis independentes:

$$IP_{MA, i} = 0,4545 \cdot P_{\text{san}, i} + 0,4545 \cdot \left( \frac{\sum_{j} \left( \frac{\text{Área } UC_{i,j}}{\text{Área } M_i} \cdot FC_j \cdot FQ_j \right)}{FCE} \right) + 0,091 \cdot \left( \frac{\text{Área Mata Seca}_i}{\text{Área } M_i} \right)$$

Este critério é altamente sensível à criação de Unidades de Conservação municipais e privadas (RPPNs) de proteção integral ($FC = 1,0$) e à eficácia de sistemas locais de tratamento de esgoto/lixo.

### 3. O Fator Redistributivo do ICMS Solidário e Mínimo Per Capita
Estes dois critérios agem em conjunto como um sistema de feedback negativo sobre a concentração de receita. Eles identificam municípios onde:

$$\frac{\sum_{k=1}^{17} IP_{k, i}}{Pop_i} < \text{Piso}$$

E calculam o complemento necessário para cobrir esse "déficit" tributário per capita. Se a soma dos repasses de todos os critérios anteriores não garantir ao cidadão local metade da média estadual de repasse, os coeficientes $IP_{17}$ e $IP_{18}$ são acionados para injetar recursos e corrigir a distorção.

---
*Documento de síntese matemática construído a partir das especificações do cofre de estudo da Lei nº 18.030/2009.*

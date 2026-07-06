---
title: População dos 50 Municípios Mais Populosos
tags:
  - criterio-repasse
  - demografia
  - populacao
  - fjp
date: 2026-07-01
weight: 2.00
---

# 🏙️ População dos 50 Municípios Mais Populosos

O critério **População dos 50 Municípios Mais Populosos** distribui **2,00%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009).

---

## 🔍 O que é este critério?

Diferente do antigo critério geral de "População" (que distribuía recursos para todos os 853 municípios com base no tamanho de sua população e que foi revogado em 2023), este critério é exclusivo para os **50 maiores centros urbanos** do Estado. 

A lei define o critério como:
> *"IV – população dos cinquenta Municípios mais populosos: relação percentual entre a população residente em cada um dos cinquenta Municípios mais populosos do Estado e a população total desses Municípios, medida segundo dados do IBGE"*

O objetivo é compensar as 50 maiores cidades do Estado pelos altos custos sociais, de saúde, segurança e infraestrutura gerados pela grande densidade e aglomeração populacional.

---

## 🧮 Fórmula de Cálculo e Estrutura das Planilhas

Para auditar os relatórios da FJP, é fundamental compreender a diferença entre o **Índice no Critério** (o valor bruto publicado nas planilhas do portal de BI) e a **Cota-Parte Ponderada no ICMS** (o impacto real na composição do IPM final).

### 1. Índice no Critério ($IC_{P50}$) - O valor da planilha da FJP
Representa a participação populacional de um município em relação à soma das populações dos 50 maiores municípios. A soma dos índices desses 50 municípios na planilha da FJP resulta em exatamente **100%** (ou **1,000000000**):

Para os municípios do grupo (Top 50):
$$IC_{P50, i} = \frac{Pop_i}{\sum_{j=1}^{50} Pop_j} \times 100\%$$

Para os demais 803 municípios de Minas Gerais:
$$IC_{P50, i} = 0\%$$

Onde:
*   $Pop_i$ = População residente no município $i$, medida segundo os dados oficiais do **IBGE**.
*   $\sum_{j=1}^{50} Pop_j$ = Soma das populações de todas as 50 maiores cidades de Minas Gerais.

### 2. Cota-Parte Ponderada no ICMS ($IP_{P50}$)
É a participação ponderada final utilizada no cálculo do IPM consolidado, obtida multiplicando-se o índice no critério pelo peso legal de **2,00%**:

$$IP_{P50, i} = IC_{P50, i} \times 2\% \text{ (ou } IC_{P50, i} \times 0,02 \text{)}$$

---

## ⚡ O Fator Crítico: O "Efeito Linha de Corte" (Top 50)

Para os municípios de médio porte, este critério possui um comportamento de **"tudo ou nada"** muito agressivo:
*   **Posição 50ª:** Recebe uma cota proporcional do repasse de 2,00% (geralmente gerando milhões de reais ao ano).
*   **Posição 51ª:** Recebe **exatamente 0%**.
*   *O Impacto:* Municípios que flutuam na zona limítrofe (entre as posições 45 e 55, como Mariana, Congonhas, Frutal, Lagoa Santa, etc.) devem auditar este índice com prioridade absoluta. Uma pequena variação na contagem populacional pode significar a entrada ou a exclusão total do rateio de 2,00% de todo o ICMS mineiro.

---

## 🔍 Como o Município Deve Auditar este Critério

O processo de auditoria deste critério divide-se em duas etapas: a conferência matemática dos dados estaduais (FJP) e a contestação dos dados demográficos de origem (IBGE).

### Fase 1: Conferência e Auditoria dos Dados Populacionais (Base IBGE)
Como a plataforma de BI da FJP exige obrigatoriamente a seleção de um município específico por vez (não permitindo o download de uma única planilha consolidada com todas as 853 cidades), a auditoria do ranking e do divisor total deve ser feita utilizando os dados de origem do **IBGE**:

1.  **Baixar a Planilha de Estimativas do IBGE:** Acesse o portal do IBGE (área de Estatísticas > População > Estimativas de População) e faça o download da planilha de Excel (`.xls` ou `.xlsx`) contendo as estimativas enviadas ao Tribunal de Contas da União (TCU) para o exercício correspondente.
2.  **Filtrar o Estado de Minas Gerais:** Abra a planilha do IBGE, localize a coluna de UF (Unidade da Federação) e filtre apenas o estado de **Minas Gerais** (código de UF `31`). Isso isolará as 853 linhas dos municípios mineiros.
3.  **Ordenar e Identificar o Top 50:** Ordene a coluna de "População Estimada" de forma decrescente. As primeiras 50 linhas corresponderão exatamente aos 50 municípios mais populosos do estado que têm direito ao repasse.
4.  **Calcular o Divisor Oficial:** Some a população dessas 50 primeiras cidades para encontrar o divisor oficial ($\sum_{j=1}^{50} Pop_j$) adotado no cálculo.
5.  **Verificar a Fração Relativa Individual:** Divida a população oficial do seu município (se estiver no grupo) pelo divisor total encontrado. O valor em percentual deve bater exatamente com o **Índice no Critério** de Lagoa Santa (ou da sua cidade correspondente) que consta no painel do portal da FJP.

### Fase 2: Auditoria e Contestação das Estimativas do IBGE (O Ponto de Ação)
Como o critério depende exclusivamente dos dados do IBGE, o município não deve contestar a FJP caso os números populacionais estejam errados, mas sim **contestar o próprio IBGE**.
*   **A Regra Federal:** De acordo com o Art. 102 da **Lei Federal nº 8.443/1992**, o IBGE publica anualmente as estimativas de população dos municípios no Diário Oficial da União (D.O.U.) até **31 de agosto**.
*   **Prazo de Contestação:** Os municípios têm um prazo improrrogável de **20 dias corridos** a contar da publicação para apresentar **reclamações e contestações fundamentadas** ao IBGE.

Se o IBGE deferir a contestação e retificar a estimativa populacional do município no Diário Oficial da União, a FJP será obrigada a utilizar o novo número na apuração definitiva do IPM para o ano seguinte.

---

## 🛠️ Como o Município Pode Melhorar o Índice
*   **Campanhas de Declaração de Domicílio:** Estimular novos moradores que se mudaram para o município a transferirem seus títulos de eleitor, cadastros de saúde e cadastros fiscais para a cidade.
*   **Preenchimento Completo do Censo:** Durante a coleta de dados de censos nacionais, estruturar equipes de apoio da prefeitura para garantir que todos os domicílios e bairros distantes sejam visitados pelos recenseadores do IBGE.

---

## 🔗 Relação com a Revogação do Critério Geral de População
Com a revogação do critério de população geral (antigo inciso III) pela Lei nº 24.431/2023, este critério específico dos 50 municípios mais populosos ganhou destaque como um dos poucos fatores de ponderação puramente demográficos restantes, concentrando o fator populacional nos grandes centros do estado (ex: Belo Horizonte, Uberlândia, Contagem, Juiz de Fora, Betim, Montes Claros, etc.).

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 1º|Art. 1º, IV]] da Lei nº 18.030/2009.*

---
title: Critério Meio Ambiente (ICMS Ecológico)
tags:
  - criterio-repasse
  - meio-ambiente
  - icms-ecologico
  - copam
  - ief
date: 2026-07-01
weight: 1.10
---

# 🌿 Critério Meio Ambiente (ICMS Ecológico)

O critério **Meio Ambiente** (popularmente conhecido como **ICMS Ecológico**) distribui **1,10%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009).

> [!tip] Impacto Ambiental e Incentivo
> Este critério premia financeiramente os municípios que investem em saneamento básico (tratamento de lixo e esgoto), na criação/manutenção de Unidades de Conservação e na preservação de biomas nativos (como a Mata Seca).

---

## 🧮 Fórmulas e Distribuição dos Recursos

Os recursos deste critério (1,10% do ICMS dos municípios) são subdivididos em três parcelas com focos distintos (Art. 4º):

$$IP_{MA, i} = (P_1 \times 45,45\%) + (P_2 \times 45,45\%) + (P_3 \times 9,10\%)$$

Onde:

---

### Partilha 1: Saneamento Básico ($P_1$) - Peso: **45,45%**
Destinada a municípios com sistemas autorizados/licenciados de tratamento ou disposição final de **Lixo** ou de **Esgoto Sanitário** que atendam, no mínimo:
*   **Lixo:** 70% da população urbana.
*   **Esgoto:** 50% da população urbana.

*   **Fator de Qualidade ($FQ_{san}$):** Varia de 0,1 a 1,0, ponderando o desempenho operacional, gestão multimunicipal (consórcios), coleta seletiva e energia gerada pelo sistema.
*   **Limite de Depreciação:** O repasse decresce 20% ao ano a partir do 11º ano do licenciamento do sistema (para incentivar a contínua modernização).

---

### Partilha 2: Unidades de Conservação e Áreas Indígenas ($P_2$) - Peso: **45,45%**
Calculada com base no **Índice de Conservação do Município ($IC_i$)** detalhado no Anexo IV da Lei:

$$IC_i = \frac{FCM_i}{FCE}$$

Onde:
*   **$FCE$ (Fator de Conservação do Estado):** $\sum_{j=1}^{853} FCM_j$
*   **$FCM_i$ (Fator de Conservação do Município $i$):** É o somatório dos fatores de conservação de cada Unidade de Conservação ($j$) presente no município:

$$FCM_i = \sum_{j} \left( \frac{\text{Área } UC_{i,j}}{\text{Área Município}_i} \times FC_j \times FQ_j \right)$$

#### Tabela de Fatores de Conservação ($FC$):
O peso do fator ($FC$) varia conforme o grau de restrição de uso da área:

| Grupo | Categoria de Manejo | Sigla | Peso ($FC$) |
| :--- | :--- | :--- | :--- |
| **Proteção Integral** | Estação Ecológica, Reserva Biológica, Parque Natural, Monumento Natural, Refúgio de Vida Silvestre | EE, RB, PAQ, MN, RVS | **1,00** |
| **Uso Sustentável** | Reserva Particular do Patrimônio Natural | RPPN | **1,00** |
| **Uso Sustentável** | Reserva Extrativista, RDS, Reserva Indígena | RESEX, REDES, AI | **0,50** |
| **APA I** | Área de Proteção Ambiental I (Zona de Vida Silvestre) | ZVS | **0,50** |
| **Uso Sustentável** | Floresta Nacional/Estadual, Reserva de Fauna, ARIE | FLO, RF, ARIE | **0,30** |
| **APA I** | Área de Proteção Ambiental I (Demais Zonas) | DZ | **0,10** |
| **Outras** | Reserva Particular de Recomposição Ambiental | RPRA | **0,10** |
| **APA II** | Área de Proteção Ambiental II | APA II | **0,025** |

*   **Fator de Qualidade ($FQ$):** Varia de 0,1 a 1,0. Avalia a infraestrutura física, plano de manejo, equipe e financiamento da Unidade (fixado em 1,0 até deliberação do Copam).

---

### Partilha 3: Mata Seca ($P_3$) - Peso: **9,10%**
Calculada pela relação percentual de área de Mata Seca (Floresta Estacional Decidual) presente no território municipal, informada pelo **Instituto Estadual de Florestas (IEF)**.

$$P_3 = \frac{\text{Área de Mata Seca}_i}{\text{Área Total do Município}_i}$$

---

## 📅 Apuração e Habilitação
*   **Habilitação Trimestral:** A **SEMAD** (Secretaria de Estado de Meio Ambiente) publica os dados constitutivos e a lista de municípios habilitados no último dia de cada trimestre civil para vigorar no trimestre subsequente.

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 4º|Art. 4º]] e [[Lei 18030-2009#ANEXO IV|Anexo IV]] da Lei nº 18.030/2009.*

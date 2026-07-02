---
title: Critério Educação
tags:
  - criterio-repasse
  - educacao
  - fundeb
  - fjp
date: 2026-07-01
weight: 10.00
---

# 🎓 Critério Educação

O critério **Educação** distribui **10,00%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009, atualizado pela Lei nº 24.431/2023).

> [!important] Novo Fundeb e EC nº 108/2020
> Este critério foi profundamente reformulado em setembro de 2023 para se alinhar à Emenda Constitucional Federal nº 108/2020, que vincula repasses de ICMS a indicadores de melhoria nos resultados de aprendizagem e de aumento da equidade na educação pública.

---

## 🧮 Fórmulas e Modelagem Matemática

O repasse individual no critério Educação para cada município é definido pelo seu **Índice de Educação ($IE_i$)**, calculado anualmente de acordo com o Anexo III da Lei:

$$IE_i = \frac{IQE_i}{\sum_{j=1}^{853} IQE_j}$$

Onde:
*   $IQE_i$ = Índice de Qualidade da Educação do município $i$.
*   $\sum_{j=1}^{853} IQE_j$ = Somatório dos índices de qualidade de educação de todos os 853 municípios do Estado.

---

### 🔍 Composição do Índice de Qualidade de Educação ($IQE_i$)

O $IQE_i$ é composto por quatro subíndices de ponderação com pesos distintos (Art. 2º, § 1º):

$$IQE_i = (IRAP_i \times 0,50) + (IRE_i \times 0,20) + (IAE_i \times 0,15) + (IGE_i \times 0,15)$$

#### 1. Índice de Desempenho Escolar ($IRAP_i$) - Peso: **50%**
Calculado com base nas avaliações externas (PROALFA/PROEB) dos estudantes do **2º, 5º e 9º anos** do Ensino Fundamental das redes municipais.
*   **Fatores de Ponderação:**
    *   Taxa de participação dos estudantes nas provas.
    *   Nível socioeconômico dos estudantes (atenuando disparidades regionais e de grupos raciais/urbanos/rurais).

#### 2. Índice de Rendimento Escolar ($IRE_i$) - Peso: **20%**
Mede o fluxo escolar e a equidade através das taxas de aprovação, de abandono e de adequação idade-série.
*   **Fatores de Ponderação:**
    *   Redução das desigualdades de acesso/permanência entre estudantes negros e não negros e urbano-rurais.
    *   Progressão de estudantes com deficiência (incluindo Transtorno do Espectro Autista - TEA).

#### 3. Índice de Atendimento Educacional ($IAE_i$) - Peso: **15%**
Apurado conforme a taxa de matrícula e atendimento nos níveis e modalidades de ensino de responsabilidade do município.
*   **Fatores de Ponderação:**
    *   Oferta de educação em tempo integral.
    *   Matrículas de estudantes quilombolas e residentes em áreas rurais.
    *   Redução da taxa de analfabetismo na população de 15 anos ou mais.

#### 4. Índice de Gestão Escolar ($IGE_i$) - Peso: **15%**
Apurado conforme dados do Censo Escolar.
*   **Fatores de Ponderação:**
    *   Infraestrutura física das escolas e acessibilidade.
    *   Formação continuada dos profissionais da educação.
    *   Efetividade da gestão democrática escolar (ex: conselhos escolares).

---

## 📅 Cronograma de Apuração

Os dados são fornecidos pela Secretaria de Estado de Educação (SEE) e calculados pela Fundação João Pinheiro (FJP):
*   **Apuração Anual:** Com base nos dados do ano civil imediatamente anterior.
*   **Publicação dos Índices:** Até o dia **31 de agosto** de cada ano.

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 2º|Art. 2º]] e [[Lei 18030-2009#ANEXO III|Anexo III]] da Lei nº 18.030/2009.*

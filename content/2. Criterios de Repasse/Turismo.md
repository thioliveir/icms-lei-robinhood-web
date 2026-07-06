---
title: Critério Turismo (ICMS Turismo)
tags:
  - criterio-repasse
  - turismo
  - setur
  - legislacao
date: 2026-07-01
weight: 0.50
---

# ✈️ Critério Turismo (ICMS Turismo)

O critério **Turismo** (ICMS Turismo) distribui **0,50%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009, atualizada pela Lei nº 24.431/2023).

> [!tip] Regulamentação por Decreto e Resolução
> O critério é regulamentado pelo **[Decreto nº 48.108/2020](https://www.almg.gov.br/legislacao-mineira/texto/DEC/48108/2020/?cons=1)** e operacionalizado pela **Resolução SECULT nº 44/2021** (que revogou expressamente a antiga Resolução SETUR nº 25/2017 em seu Art. 47).

---

## 📋 Regras de Habilitação e Habilitação Preliminar

Para se habilitar ao recebimento dos repasses do ICMS Turismo, o município deve atender cumulativamente a quatro requisitos mínimos (Art. 3º do Decreto):
1.  **Participação em IGR:** Participar do Programa de Regionalização do Turismo da SECULT, integrando uma *Instância de Governança Regional (IGR)* certificada.
2.  **Política Municipal de Turismo:** Possuir e comprovar a implementação de uma Política Municipal de Turismo.
3.  **COMTUR (Conselho Municipal de Turismo):** Possuir e manter em regular funcionamento o Conselho.
4.  **FUMTUR (Fundo Municipal de Turismo):** Possuir e manter em regular funcionamento o Fundo.

---

## 🧮 Funcionamento do Cálculo ($IP_{TU}$)

O repasse de cota-parte individual de cada município habilitado baseia-se na ponderação do seu esforço de investimento em turismo pelo inverso de sua receita corrente líquida per capita, conforme estabelece o Anexo VI da Lei nº 18.030/2009.

### Passo 1: Cálculo da Pontuação Ponderada do Município
Para cada município ($i$), multiplica-se a nota técnica de sua organização turística pelo peso da sua receita per capita:

$$\text{Pontuação Ponderada}_i = \text{NT}_i \times \text{IRC}_i$$

Onde:
*   **$\text{NT}_i$ (Nota da Organização):** Pontuação de 0 a 10 atribuída pela SECULT à documentação do município (COMTUR, FUMTUR, IGR, política local).
*   **$\text{IRC}_i$ (Fator de Receita):** Multiplicador (peso de 1 a 10) inversamente proporcional à Receita Corrente Líquida (RCL) per capita da cidade. Promove a equidade fiscal ao dar pesos maiores para municípios com menor receita própria.

### Passo 2: Cálculo do Índice de Investimento em Turismo ($\text{IIT}$)
O $\text{IIT}_i$ representa o percentual de participação do município sobre a pontuação ponderada somada de **todos** os municípios habilitados no Estado:

$$\text{IIT}_i = \frac{\text{NT}_i \times \text{IRC}_i}{\sum_{j} (\text{NT}_j \times \text{IRC}_j)}$$

### Passo 3: Índice de Participação Final ($IP_{TU}$)
O repasse final do município ($IP_{TU, i}$) é a aplicação do $\text{IIT}_i$ sobre o percentual total destinado ao critério (0,50% do ICMS dos municípios):

$$IP_{TU, i} = \text{IIT}_i \times 0,50\%$$

---

## 📊 Estudo de Caso Real: Exercício 2026 (Ano-Base 2024)

Para entender a aplicação prática da fórmula, tomemos como exemplo o caso real do município de **Abaeté** (integrante do Circuito Turístico Lago de Três Marias) publicado nos índices definitivos de 2026:

*   **Nota Técnica ($\text{NT}$):** `10,00` (Abaeté cumpriu com êxito todas as exigências e atingiu nota máxima).
*   **Receita Per Capita (RCL):** R$ `4.629,36`.
*   **Fator de Receita ($\text{IRC}$):** `8` (Faixa de enquadramento da FJP para essa receita).
*   **Pontuação Ponderada ($\text{NT} \times \text{IRC}$):**
    $$\text{Pontuação Ponderada} = 10,00 \times 8 = 80,00$$
*   **Soma do Estado ($\sum (\text{NT} \times \text{IRC})$):** `5.979,07` (Soma das bases de todas as cidades habilitadas em MG).
*   **Índice de Investimento em Turismo ($\text{IIT}$):**
    $$\text{IIT}_{\text{Abaeté}} = \frac{80,00}{5.979,07} \approx 0,013380$$
*   **Índice Definitivo de Participação ($IP_{TU}$):**
    Devido às regras de normalização do ano fiscal e ao número total de habilitados concorrentes, o índice final pago ao município é escalonado em relação ao bolo geral dos repasses:
    $$IP_{TU, \text{Abaeté}} \approx 0,013380 \times 18,17638 \approx \mathbf{0,243200\%}$$

---

## 📅 Calendário e Prazos do Sistema

Todo o envio de dados é eletrônico e gerenciado através do **[Sistema do ICMS Turismo](http://www.icmsturismo.mg.gov.br)**:
*   **Até 1º de Março (Meta Anual):** Prazo final improrrogável para inserção e fechamento de toda a documentação comprobatória do ano-base anterior no sistema (Art. 11 da Resolução nº 44/2021).
*   **Até 15 de Julho:** Divulgação dos Índices Provisórios.
*   **Até 15 de Agosto:** Divulgação dos Índices Definitivos.

---

## 🔍 Como o Município Deve Auditar o Critério

O ICMS Turismo possui um dos ritos documentais mais exigentes do ICMS Solidário, demandando atenção aos seguintes itens de auditoria:

### 1. Rigor nas Atas do COMTUR (Art. 25 e 26 da Resolução nº 44/2021)
*   **Identificação de Participantes:** As atas de reunião do COMTUR devem ser digitalizadas em PDF contendo, obrigatoriamente, o nome de todos os conselheiros presentes, o nome dos ausentes e a assinatura física/digital de todos os participantes.
*   **Proibição de Atas Exclusivamente Administrativas:** Atas que tratem apenas de posses de membros, eleições de mesa diretora ou mudanças de regulamento **não serão computadas** para a periodicidade mínima do conselho. As atas devem debater e deliberar sobre as ações reais de fomento ao turismo municipal.
*   **Relatório Anual Obrigatório:** O Relatório de Atividades do COMTUR deve ser preenchido na última reunião do ano-base, registrando em ata a participação e concordância dos conselheiros com os dados declarados.

### 2. Validação do Plano Municipal de Turismo (Art. 17)
*   O Plano de Turismo deve ter vigência comprovada. Caso o plano tenha sido aprovado em uma gestão anterior do conselho e não possua ata formal de aprovação da época, a gestão atual do COMTUR deve realizar uma reunião específica para **validar o plano vigente**, registrando a aprovação formal em ata.

### 3. Prestação de Contas do FUMTUR (Art. 28 a 33)
*   **Exclusividade da Conta:** Exige-se ofício assinado pelo Prefeito atestando a titularidade e a exclusividade da conta bancária individualizada do FUMTUR, com dados de agência e conta corrente.
*   **Confronto Bancário:** O auditor municipal deve validar se o extrato bancário anual bate exatamente com os créditos e débitos inseridos no sistema.
*   **Declaração Quádrupla de Regularidade:** O município deve enviar uma declaração conjunta assinada por **4 pessoas**: o Prefeito, o Gestor do Fundo e **2 (dois) conselheiros do COMTUR**, atestando que todas as movimentações e saídas de despesas do fundo seguiram a lei municipal de turismo e foram voltadas para investimentos com finalidade exclusivamente turística.
*   **Comprovantes Inequívocos (Glosas):** Todas as despesas do FUMTUR devem ser comprovadas por notas fiscais ou notas de empenho que demonstrem a finalidade turística. A prova não pode ser feita por atas.

### 4. Notificações e Prazo de Recurso (15 Dias)
*   **Correções de Omissão (10 dias):** Caso a comissão técnica aponte inconformidades, o gestor terá **10 dias corridos** para realizar retificações.
*   **Impugnação de Índices Provisórios:** O prazo para prefeitos ou associações apresentarem recursos contra os índices provisórios publicados é de **15 dias corridos** após a divulgação (Art. 39).
*   **Guarda por 5 Anos:** Toda a documentação e extratos do FUMTUR devem ser guardados em arquivo por 5 anos a contar do encerramento do sistema.

---
*Documento de estudo com base no **[Decreto nº 48.108/2020](https://www.almg.gov.br/legislacao-mineira/texto/DEC/48108/2020/?cons=1)**, na **Resolução SECULT nº 44/2021** (que revogou a Resolução SETUR nº 25/2017), e na Lei nº 18.030/2009.*

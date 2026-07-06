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

## 🧮 Fórmulas e Modelagem Matemática (Resolução Conjunta SEE/FJP nº 13/2024)

O repasse individual da cota-parte da Educação ($IE_i$) de cada município baseia-se no seu **Índice de Qualidade da Educação ($IQE_i$)** apurado relativamente aos dados do ano anterior:

$$IE_i = \frac{IQE_i}{\sum_{j=1}^{853} IQE_j} \times 10\%$$

Onde o **Índice de Qualidade da Educação ($IQE_i$)** é composto por quatro subíndices com os seguintes pesos regulamentares:

$$IQE_i = (IDE_i \times 0,50) + (IRE_i \times 0,20) + (IAE_i \times 0,15) + (IGE_i \times 0,15)$$

---



### 1. Índice de Desempenho Escolar ($IDE_i$) — Peso: **50%**
Mede o aprendizado dos estudantes do **2º, 5º e 9º anos** do Ensino Fundamental (com pesos internos de 40%, 40% e 20%):
*   **50%** do índice baseia-se no percentual de estudantes nos níveis **Recomendado e Avançado** nas avaliações do **Simave (PROALFA/PROEB)**, ponderado pela taxa de participação da escola e pelo **Índice de Vulnerabilidade** do município.
*   **50%** do índice baseia-se na razão entre a proficiência real (Língua Portuguesa e Matemática) e o **Desempenho Esperado** (calculado via regressão linear baseada no Nível Socioeconômico - NSE divulgado pelo INEP).

### 2. Índice de Rendimento Escolar ($IRE_i$) — Peso: **20%**
Avalia o fluxo dos estudantes do **5º e 9º anos** (pesos de 80% e 20%):
*   Consiste na média simples entre a **Taxa de Aprovação**, **Taxa de Abandono (1 - Abandono)** e a **Taxa de Distorção Idade-Série (1 - Distorção)** (dados publicados pelo INEP).
*   O resultado é multiplicado pelo **Índice de Vulnerabilidade**, pelo **Fator de Porte da Rede Municipal** (que varia de 0,55 para menos de 500 matrículas a 1,00 para mais de 15.000 matrículas) e ponderado pelo percentual de alunos da **Educação Especial** ($1 + \text{EstudantesDeficiência}$).

### 3. Índice de Atendimento Educacional ($IAE_i$) — Peso: **15%**
Apurado conforme os dados de matrículas declarados no Censo Escolar:
*   **45%:** Proporção de alunos de 5º e 9º anos matriculados na rede municipal em relação ao total da rede pública (municipal + estadual + federal) na cidade.
*   **30%:** Total de matrículas de Educação Infantil (EI) e Ensino Fundamental (EF) do município em relação ao somatório de matrículas de todos os municípios do estado.
*   **20%:** Proporção de alunos matriculados em regime de **Tempo Integral** na rede municipal.
*   **5%:** Proporção de alunos matriculados na EJA/EF na rede municipal em relação ao total público da cidade.

### 4. Índice de Gestão Escolar ($IGE_i$) — Peso: **15%**
Mede a eficiência administrativa e a infraestrutura das escolas:
*   **40% (Formação Docente):** Proporção de professores do Ensino Fundamental com formação adequada à área em que lecionam (AFD - INEP).
*   **40% (Infraestrutura):** Média da proporção de escolas ativas que possuem: Acessibilidade (25%), Água Potável (25%), Esgoto Sanitário (25%) e Internet para fins pedagógicos (25%).
*   **20% (Gestão Democrática):** Proporção de escolas municipais que selecionam diretores combinando **processo seletivo qualificado** (prova de competências) e **eleição** com participação da comunidade.

---

## 🔍 Como o Município Deve Auditar o Critério Educação

Por envolver diversas bases de dados externas e cruzamentos complexos da SEE/MG e do INEP, os municípios devem auditar este critério com atenção metodológica extrema. O ponto de partida é baixar a planilha detalhada de cálculo anual, disponibilizada na aba **[Documentos da Lei Robin Hood - FJP](https://robin-hood.fjp.mg.gov.br/documentos)**.

---

## 🛠️ Diagnóstico e Oportunidades de Melhoria por Subíndice

Utilizando a planilha detalhada da FJP, o município deve realizar o diagnóstico de cada indicador:

### 1. Desempenho Escolar ($IDE_i$) — Foco: SIMAVE/Proeficiência
*   **Onde buscar os dados de origem:** Os resultados das provas de Língua Portuguesa e Matemática e a taxa de participação estão disponíveis no portal do **[SIMAVE (Secretaria de Estado de Educação de MG)](https://simave.educacao.mg.gov.br/#!/plataforma)**.
*   **⚠️ Regra do Quórum Mínimo:** Conforme regulamento próprio do SIMAVE, a escola municipal só terá seus resultados de proficiência divulgados e contabilizados pela FJP se atingir o **mínimo de 80% de participação dos estudantes matriculados** na série avaliada (2º, 5º e 9º anos) no dia da prova. 
    *   *Diagnóstico:* Se a coluna `taxa_participacao_simave` na planilha da FJP estiver abaixo de `0.80`, os resultados daquela turma são descartados (zerados) no cálculo.
    *   *Melhoria:* Criar mutirões de conscientização familiar e transporte escolar especial nos dias das avaliações do Simave para garantir a presença em massa dos alunos.

### 2. Rendimento Escolar ($IRE_i$) — Foco: Fluxo e Equidade
*   **Onde buscar os dados de origem:** As taxas são publicadas e detalhadas nos seguintes links específicos do INEP:
    *   **Taxas de Rendimento Escolar (Aprovação/Abandono):** [INEP - Taxas de Rendimento](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/taxas-de-rendimento-escolar)
    *   **Taxas de Distorção Idade-Série:** [INEP - Taxas de Distorção](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/taxas-de-distorcao-idade-serie)
*   **Como diagnosticar na planilha:** Abra a aba `Rendimento` e cruze os dados das colunas `taxa_aprovacao`, `taxa_abandono` e `taxa_distorcao` com os relatórios internos da rede municipal. 
    *   *Melhoria:* Implementar aulas de reforço escolar e busca ativa para reduzir o abandono (evasão), além de programas de promoção de fluxo para corrigir a distorção idade-série.

### 3. Atendimento Educacional ($IAE_i$) — Foco: Matrículas e Tempo Integral
*   **Onde buscar os dados de origem:** Os quantitativos de matrículas gerais e em tempo integral podem ser visualizados no **[Painel Inep Data (Estatísticas do Censo Escolar)](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/inep-data/estatisticas-censo-escolar)**.
*   **Como diagnosticar na planilha:** Na aba `Atendimento`, audite a coluna `matriculados_tempo_integral` para verificar se todas as turmas que estudam 7 horas ou mais por dia foram computadas.
    *   *Melhoria:* Expandir os convênios ou a oferta própria de turmas de **Tempo Integral** na Educação Infantil e Ensino Fundamental municipal (aumenta o indicador `percentual_tempo_integral` que representa 20% deste subcritério).

### 4. Gestão Escolar ($IGE_i$) — Foco: Formação, Infraestrutura e Gestão Democrática
*   **Onde buscar os dados de origem:** Também pode ser visualizado no **[Painel Inep Data (Estatísticas do Censo Escolar)](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/inep-data/estatisticas-censo-escolar)**.
*   **Como diagnosticar na planilha (Aba `Gestão`):**
    *   **Formação Docente ($iGE\_AFDi$):** Verifique o percentual na coluna `proporcao_docentes_formacao_adequada_ef`. O indicador oficial de referência pode ser consultado no portal de **[Adequação da Formação Docente do INEP](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/adequacao-da-formacao-docente)**.
        *   *Melhoria:* Ofertar programas de capacitação continuada e incentivos para que os docentes obtenham a licenciatura adequada para as áreas e disciplinas específicas em que lecionam no Ensino Fundamental.
    *   **Gestão Democrática ($iGE\_GDi$):** Verifique se o município recebeu pontuação zero na coluna `escolas_selecionam_diretores_qualificado`.
        *   *Melhoria:* Regulamentar por lei municipal a seleção de diretores de escolas que combine **processo seletivo de prova técnica** (processo qualificado) com a subsequente **eleição da comunidade escolar**, garantindo a pontuação integral deste subcritério (20% do índice de gestão).
    *   **Infraestrutura ($iGE\_IEi$):** Verifique se todas as escolas ativas possuem acessibilidade, água potável, esgotamento sanitário (fossa ou rede pública) e internet para fins de ensino.
        *   *Melhoria:* Realizar investimentos focados na melhoria desses 4 serviços nas escolas pendentes e, crucialmente, orientar os secretários escolares para **declararem essas infraestruturas corretamente** durante o Censo Escolar em maio.

---

## 📅 Cronograma de Apuração e Recursos

### 🗓️ Calendário de Coleta e Retificação do Censo Escolar (INEP)
Como o Censo Escolar não possui um portal estatístico com números vivos durante o processo (sendo publicado e retificado via Diário Oficial da União - DOU), o município deve acompanhar rigidamente o cronograma nacional:

*   **Data de Referência do Censo Escolar:** Última quarta-feira de maio (ex: **27/05/2026**).
*   **Período de Coleta e Inserção de Dados:** De maio a julho (ex: **27/05/2026 a 31/07/2026**).
*   **Publicação dos Resultados Preliminares (DOU):** 1ª quinzena de setembro (previsão).
*   **⚠️ Janela Crítica de Retificação (Prazo de 30 dias):** O município tem o prazo máximo de **30 dias corridos** após a publicação preliminar no DOU para conferir os dados e retificar quaisquer erros de declaração de infraestrutura, matrículas ou diretores diretamente no sistema do Censo Escolar. *Decorrido esse prazo, as informações são consolidadas de forma definitiva e enviadas à FJP, não sendo mais passíveis de alteração.*
*   **Publicação dos Resultados Finais (DOU):** 1ª quinzena de fevereiro do ano seguinte (previsão).
*   **Divulgação das Sinopses Estatísticas da Educação Básica:** Início de fevereiro (ex: **01/02/2027**).

### 🗓️ Cronograma FJP (Apuração do ICMS)
*   **15 de Agosto:** Prazo limite para a Secretaria de Estado de Educação (SEE/MG) enviar os dados escolares consolidados para a Fundação João Pinheiro.
*   **31 de Agosto:** A FJP publica em seu sítio eletrônico os índices provisórios de participação de cada município no critério Educação.
*   **Impugnação de Índices:** Se o município identificar na planilha da FJP divergências em relação aos dados finais do DOU/Simave, deve protocolar recurso de impugnação em até **30 dias** após a publicação provisória. O julgamento e os resultados das impugnações definitivas devem ser publicados pela FJP em até **15 dias** após o encerramento do prazo de recebimento.

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 2º|Art. 2º]] da Lei nº 18.030/2009 e na Resolução Conjunta SEE/FJP nº 13/2024.*

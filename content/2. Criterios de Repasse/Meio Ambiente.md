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

### Partilha 1: Saneamento Básico ($P_1$) — Peso: **45,45%**
Destinada a municípios com sistemas autorizados/licenciados de tratamento ou disposição final de **Resíduos Sólidos (Lixo)** ou de **Esgoto Sanitário** (conforme a classificação de tipologia licenciável da **[Deliberação Normativa COPAM nº 217/2017](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=45558)**) que atendam aos seguintes percentuais mínimos de cobertura urbana:
*   **Resíduos Sólidos (Lixo):** No mínimo **70%** da população urbana atendida.
*   **Esgoto Sanitário:** No mínimo **50%** da população urbana atendida.

*   **Fator de Qualidade ($FQ_{san}$):** A apuração do Fator de Qualidade baseia-se no tipo de empreendimento, eficiência operacional e atendimento populacional:
    *   *Regulação:* Regido pelas diretrizes da **[Resolução Conjunta SEMAD-SEPLAG nº 1.212/2010](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=14931)** e metodologias da **[Resolução SEMAD nº 1.273/2011](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=16214)**, as quais são complementadas e atualizadas pela **[Resolução SEMAD nº 3.371/2025](https://www.pesquisalegislativa.mg.gov.br/LegislacaoCompleta.aspx?cod=216310&marc=)**. 
    *   *Pontuação e Primeiro Cadastro:* O $FQ$ varia em uma faixa de **0,05 a 1,0**. No primeiro ano de cadastramento do sistema, o município recebe automaticamente a nota máxima de **1,0**. Nos anos subsequentes, essa pontuação é recalculada conforme o desempenho ambiental do município.
    *   *Relatório Anual Obrigatório (Prazo Limite: 31 de Março):* Para apuração do Fator de Qualidade, a prefeitura deve enviar anualmente à SEMAD, até o dia **31 de março**, o *Relatório de Apuração do Fator de Qualidade* com informações do ano-base anterior. A documentação e formulários necessários estão disponíveis na página oficial de **[Formulários e Material de Apoio - Fator de Qualidade SEMAD](https://meioambiente.mg.gov.br/web/semad/fator-de-qualidade)**.
    *   *Os 4 Eixos de Avaliação:*
        1.  **Gestão do Passivo Ambiental ($GPA$):** Avaliação de passivos, recuperação de áreas e conformidades ambientais.
        2.  **Desempenho Operacional ($DOP$):** Operação técnica adequada do aterro sanitário ou da estação de tratamento.
        3.  **Gestão de RSU / Aproveitamento Energético ($GRS$):** Redução na geração de resíduos e aproveitamento energético (biogás, etc.).
        4.  **Coleta Seletiva e Organização ($CSO$):** Projetos de coleta seletiva e apoio a associações de catadores de materiais recicláveis.
    *   *Investimentos Referenciais:* A **Deliberação COPAM nº 230/2018** fixa os parâmetros per capita para estimativas de custos de implantação/investimento dos sistemas.
*   **Limite de Depreciação:** Como incentivo à contínua modernização, o repasse financeiro do sistema licenciado decresce **20% ao ano** a partir do 11º ano de concessão/operação do licenciamento ambiental.

---

### Partilha 2: Unidades de Conservação e Áreas Indígenas ($P_2$) — Peso: **45,45%**
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

*   **Fator de Qualidade da Unidade ($FQ_j$):** Varia de 0,1 a 1,0. É a nota recebida pela gestão da UC (infraestrutura, equipe, conselho, plano de manejo) apurada anualmente pelo órgão gestor, conforme critérios da **[Deliberação Normativa COPAM nº 234/2019](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=49401)**. O cadastramento municipal de UCs deve seguir os requisitos da **[Resolução SEMAD nº 318/2005](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=4167)** e **Resolução SEMAD nº 1.245/2010**.

---

### Partilha 3: Mata Seca ($P_3$) — Peso: **9,10%**
Destinada a recompensar os municípios que possuem cobertura florestal do bioma Mata Seca (Floresta Estacional Decidual no bioma Cerrado) sem associação com cursos d'água.
*   **Como é calculado:** É o resultado do cruzamento entre o *Mapeamento da Cobertura Vegetal e de Reflorestamentos de Minas Gerais (2009)* e as supressões detectadas anualmente pelo programa de *Monitoramento Contínuo* do IEF.
*   **Habilitação:** Automática, calculada pela Gerência de Monitoramento Territorial e Geoinformação (GEMOG) do IEF.

---

## 🔍 Como o Município Deve Auditar o Critério

Os dados consolidados de habilitação de cada município são publicados trimestralmente na página oficial da **[SEMAD - ICMS Ecológico](https://meioambiente.mg.gov.br/web/semad/icms-ecologico-publicacoes)**. O auditor municipal deve atuar ativamente nas três frentes de controle financeiro e documental:

### 1. Auditoria de Saneamento Básico (ISA)
*   **⚠️ Risco de Exclusão Sem Retroativo:** É de responsabilidade exclusiva do município manter o cadastro atualizado perante a SEMAD. Caso o cadastro seja desabilitado por atraso ou erro documental (ex: licença vencida ou contrato de disposição vencido), o município **não terá direito a receber retroativamente** os repasses do período de inatividade.
*   **Gatilhos Obrigatórios de Atualização cadastral:** O cadastro deve ser retificado via SEI! sempre que ocorrer:
    *   Vencimento ou aditamento de contratos de disposição final.
    *   Alteração da destinação (mudança de aterro/UTC).
    *   Vencimento da licença ambiental do aterro sanitário ou da ETE.

#### 📁 Processo de Cadastro Inicial e Atualizações no SEI!MG
O cadastramento deve ser realizado **exclusivamente** de forma eletrônica através do sistema **SEI!MG 4.0** (Peticionamento Eletrônico - Usuário Externo). Não são aceitos envios físicos por Correios, ofícios impressos ou e-mails.
*   **Tipo de Processo:** Selecionar `Semad - ICMS ecológico - Resíduos Sólidos Urbanos`.
*   **Checklist Documental Obrigatório:**
    1.  *Formulário SEMAD – ICMS Ecológico – Resíduos Sólidos Urbanos* (gerado eletronicamente no SEI).
    2.  *Contrato de Disposição Final de RSU:* Cópia do contrato ou convênio ativo com o aterro/UTC (se estiver vencido, o cadastro é recusado de imediato).
    3.  *Contratos de Consórcios:* Contratos de rateio e de programa, caso o município destine via consórcio intermunicipal.
    4.  *Contratos de Transporte Terceirizado:* Caso contrate transportadora intermediária, deve apresentar o contrato que comprove o vínculo da transportadora com o aterro licenciado de destino.
    5.  *Cópia da Licença Ambiental:* Do empreendimento de tratamento/disposição final de RSU.

*   **Canais de Consulta e Retificação (Saneamento):**
    *   *Resíduos Sólidos (Lixo):* Diretoria de Resíduos Sólidos Urbanos da SEMAD. Telefone: `(31) 3915-1131` | E-mails: `icms.rsu@meioambiente.mg.gov.br` (preferencial), `drsu.semad@meioambiente.mg.gov.br` ou `rafael.freitas@meioambiente.mg.gov.br`.
    *   *Esgotamento Sanitário:* Diretoria de Abastecimento de Água e Esgotamento Sanitário da SEMAD. Telefone: `(31) 3915-1223` | E-mail: `rodrigo.cevidanes@meioambiente.mg.gov.br`.

### 2. Auditoria do Índice de Conservação (IC)
*   **Auditar Cadastro de UCs:** Verificar no IEF se as UCs municipais criadas foram devidamente cadastradas com base no checklist do *Manual de Procedimentos para Cadastramento de Unidades de Conservação*.
*   **Auditar o Fator de Qualidade ($FQ_j$):** Entregar anualmente a documentação de gestão da UC exigida pela DN COPAM nº 234/2019 para garantir nota 1,0. A omissão de dados derruba o fator e reduz o repasse.
    *   *Setor de Contato (IEF):* Diretoria de Áreas Protegidas do IEF. Telefones: `(31) 3915-1710` ou `(31) 3915-2810`.

### 3. Auditoria de Mata Seca (IMS)
*   **Mapeamento de Supressão:** Se o município discordar das detecções de desmatamento automático registradas pelo IEF que reduziram sua área de Mata Seca:
    *   *Setor de Contato (IEF):* Gerência de Monitoramento Territorial e Geoinformação (GEMOG). Telefone: `(31) 3915-1363` | E-mail: `gemog.ief@meioambiente.mg.gov.br`.

---

## 📅 Calendário de Prazos e Habilitação Trimestral

Embora as prefeituras possam protocolar a documentação a qualquer momento do ano, a SEMAD consolida os cadastros de forma trimestral. O envio incompleto ou atrasado adia a apuração para o trimestre subsequente:

| Janela Trimestral | Prazo Limite para Envio no SEI! | Início do Repasse Financeiro |
| :--- | :--- | :--- |
| **1ª Habilitação Trimestral** | Último dia útil de **Janeiro** | A partir de **Abril** |
| **2ª Habilitação Trimestral** | Último dia útil de **Abril** | A partir de **Julho** |
| **3ª Habilitação Trimestral** | Último dia útil de **Julho** | A partir de **Outubro** |
| **4ª Habilitação Trimestral** | Último dia útil de **Outubro** | A partir de **Janeiro** |

> [!important] Prazo do Fator de Qualidade ($FQ_{san}$)
> O prazo para envio do Relatório de Apuração do Fator de Qualidade (RSU) é fixo e anual: até **31 de março** de cada ano. O não envio ou informações errôneas geram a perda imediata de até **57,50%** da pontuação de responsabilidade municipal.

---

## 📈 Estudo de Caso Real: Exercício 2026 (Ano-Base 2025)

Como exemplo prático de aplicação e oportunidades de auditoria, a tabela abaixo compara os dados oficiais homologados pelas **[Resoluções SEMAD nº 3.405/2026](https://semad.mg.gov.br/documents/d/semad/tabela-pontuacao-final-fq-2025-pdf)** (Fator de Qualidade de UCs) e **[nº 3.406/2026](https://semad.mg.gov.br/documents/d/semad/tabelas-referentes-as-resolucoes-icms-ecologico-5-pdf)** (Saneamento Ambiental e Índices Finais) para dois municípios distintos:

| Indicador / Subcritério                      | Abadia dos Dourados (IBGE: 10)                   | Lagoa Santa (IBGE: 3760)                     |
| :------------------------------------------- | :----------------------------------------------- | :------------------------------------------- |
| **População Urbana** (Censo)                 | 5.853 habitantes                                 | 22.945 habitantes (área UC)                  |
| **Sistemas LO/AAF Cadastrados**              | 1 Aterro Sanitário (AS RSU) - 100% pop. atendida | Nenhum sistema cadastrado/habilitado         |
| **Estimativa de Investimento (RSU)**         | R$ 187.296,00 (k = 40)                           | R$ 0,00                                      |
| **Índice de Saneamento ($Isa_{Final}$)**     | **0,00205804**                                   | **0,00000000**                               |
| **Índice de Conservação ($IC_i$)**           | **0,00000000** (Zero UCs cadastrados)            | **0,00863477** (4 UCs cadastradas)           |
| **Índice de Mata Seca ($IMS_i$)**            | **0,00000000** (Sem ocorrência de Mata Seca)     | **0,00000000** (Sem ocorrência de Mata Seca) |
| **Índice Final Consolidado ($IMA_i$)**       | **0,0009354**                                    | **0,0039245**                                |
| **Percentual FJP (%) de Repasse** (Julho/26) | **0,130005721%**                                 | **0,388849952%**                             |

> [!note] Entendendo a Diferença entre o Índice SEMAD ($IMA_i$) e o Percentual FJP (%)
> É comum observar que os valores do **Índice Final ($IMA_i$)** da SEMAD não guardam uma proporção idêntica ou direta com o **Percentual de Repasse** da FJP para o mês julho/26. Isso decorre de dois motivos regulatórios fundamentais:
> 1. **Defasagem Temporal de Pagamento (Ano-Base vs. Exercício):** As resoluções de indicadores da SEMAD apuradas em um ano (ex: dados de **2025** consolidando UCs e aterros) representam o **Ano-Base 2025**, que será pago apenas no **Exercício de 2027**. O percentual que o município recebe na conta em **Julho de 2026** é fruto dos dados do **Ano-Base 2024** (Exercício 2026).
> 2. **Cálculo de Proporção Estadual (Cota-Parte):** O percentual de repasse municipal de um critério específico é a cota-parte do município em relação à soma de todos os índices do estado:
>    $$\text{Percentual do Critério}_i = \frac{IMA_i}{\sum_{j=1}^{853} IMA_j} \times 100\%$$
>    Como a situação operacional dos outros 851 municípios mineiros oscila a cada ano, a soma estadual ($\sum IMA$) se altera, modificando a distribuição percentual mesmo se o índice individual da cidade ficar estático.

### 🔍 Oportunidades de Auditoria e Incremento de Receita:

#### 1. Abadia dos Dourados (Foco em Conservação)
*   **Diagnóstico:** O município pontua bem no saneamento devido ao seu aterro sanitário regularizado ($Isa_{Final} = 0,00205804$), mas a sua nota de conservação é nula.
*   **Plano de Ação:** O auditor municipal deve incentivar proprietários rurais a criarem **Reservas Particulares do Patrimônio Natural (RPPNs)**, que possuem peso de conservação $FC = 1,0$. Outra alternativa é a criação de uma **APA Municipal** regulamentada e com conselho consultivo ativo para pontuar no subcritério de Unidades de Conservação.

#### 2. Lagoa Santa (Foco em Saneamento e Gestão de UCs)
*   **Diagnóstico de Saneamento:** Embora possua infraestrutura urbana, o município pontua **zero** no saneamento por não possuir sistemas de lixo ou esgoto regularizados no SEI!. A ativação de um cadastro de RSU habilitado elevaria imediatamente o $IMA$ municipal.
*   **Diagnóstico de Conservação ($IC$):** O município pontua apenas graças às suas 4 Unidades de Conservação, porém os **Fatores de Qualidade ($FQ$)** homologados na **[Resolução SEMAD nº 3.405/2026](https://semad.mg.gov.br/documents/d/semad/tabela-pontuacao-final-fq-2025-pdf)** estão muito abaixo do potencial máximo de 1,0:
    *   *APA Federal Carste Lagoa Santa:* $FC = 0,5$ \| $FQ = 0,48$ (Regular)
    *   *RVS Estadual Macaúbas:* $FC = 1,0$ \| $FQ = 0,08$ (Crítico)
    *   *Parque Estadual do Sumidouro:* $FC = 1,0$ \| $FQ = 0,71$ (Bom)
    *   *Monumento Natural Estadual Várzea da Lapa:* $FC = 1,0$ \| $FQ = 0,16$ (Crítico)
*   **Plano de Ação:** A prefeitura deve colaborar ativamente com os conselhos gestores e órgãos estaduais (IEF) para estruturar a gestão dessas UCs (implementando plano de manejo, equipe técnica estável e infraestrutura de visitação). Aumentar os $FQ$ para **1,0** triplicaria a pontuação do município nesse indicador, gerando expressivo retorno financeiro anual.

---

## 📊 Consulta de Repasses Financeiros
Os valores repassados e os índices municipais do ICMS Ecológico podem ser auditados no portal oficial da Fundação João Pinheiro (FJP):
*   **Consulta de Extrato por Município:** **[FJP - Repasses Robin Hood](http://robin-hood.fjp.mg.gov.br/municipios)**
*   **Perguntas Frequentes (FAQ):** **[FJP - FAQs](http://robin-hood.fjp.mg.gov.br/faqs)**
*   **Suporte e Contatos da FJP:** **[FJP - Contatos](http://robin-hood.fjp.mg.gov.br/contatos)**

---
*Documento de estudo com base no Art. 4º e Anexo IV da Lei nº 18.030/2009, Resoluções SEMAD [nº 318/2005](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=4167), [nº 1.212/2010](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=14931), [nº 1.273/2011](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=16214), [nº 3.371/2025](https://www.pesquisalegislativa.mg.gov.br/LegislacaoCompleta.aspx?cod=216310&marc=) e Deliberações Normativas COPAM [nº 217/2017](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=45558), nº 230/2018 e [nº 234/2019](https://www.siam.mg.gov.br/sla/download.pdf?idNorma=49401). Mais informações no portal oficial da **[Secretaria de Estado de Meio Ambiente e Desenvolvimento Sustentável - SEMAD](https://meioambiente.mg.gov.br/web/semad/icms-ecologico-criterios)**.*

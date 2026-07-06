---
title: Critério Patrimônio Cultural
tags:
  - criterio-repasse
  - cultura
  - patrimonio-historico
  - iepha
date: 2026-07-01
weight: 1.00
---


# 🏛️ Critério Patrimônio Cultural

O critério **Patrimônio Cultural** distribui **1,00%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009).

> [!note] Pioneirismo de Minas Gerais
> Minas Gerais foi o primeiro estado do Brasil a incluir a preservação do patrimônio histórico e cultural como critério de repasse do ICMS, incentivando os municípios a criarem conselhos, fundos e leis de tombamento locais.

---

## 🧮 Fórmula de Cálculo ($IP_{PC}$)

O repasse individual no critério Patrimônio Cultural para cada município é definido pelo seu **Índice de Patrimônio Cultural ($PPC_i$)**, calculado anualmente de acordo com o Anexo II da Lei:

$$PPC_i = \frac{\text{Nota do Município}_i}{\sum_{j=1}^{853} \text{Nota do Município}_j}$$

Onde:
*   **$\text{Nota do Município}_i$** = Somatório das notas dos atributos de patrimônio cultural alcançados pelo município $i$, validados pelo **IEPHA-MG** (Instituto Estadual do Patrimônio Histórico e Artístico).
*   **$\sum_{j=1}^{853} \text{Nota do Município}_j$** = Somatório de todas as notas obtidas por todos os 853 municípios do Estado.

---

## 📋 Tabela de Pontuação por Atributo (Anexo II)

A pontuação do município é cumulativa e considera bens protegidos em nível federal, estadual e municipal:

| Atributo / Característica | Sigla | Pontuação (Nota) |
| :--- | :--- | :--- |
| **Núcleo Histórico Tombado (Estadual ou Federal)** | | |
| *   Até 2.000 domicílios | NH e/f 05 | **5** |
| *   De 2.001 a 3.000 domicílios | NH e/f 08 | **8** |
| *   De 3.001 a 5.000 domicílios | NH e/f 12 | **12** |
| *   Acima de 5.000 domicílios | NH e/f 16 | **16** |
| **Conjuntos Urbanos/Paisagísticos Tombados (Estadual/Federal)** | | |
| *   Área de 0,2 a 1,9 ha ou com 5 a 10 unidades | CP e/f 02 | **2** |
| *   Área de 2 a 4,9 ha ou com 11 a 20 unidades | CP e/f 03 | **3** |
| *   Área de 5 a 10 ha ou com 21 a 30 unidades | CP e/f 04 | **4** |
| *   Área acima de 10 ha ou com mais de 30 unidades | CP e/f 05 | **5** |
| **Bens Imóveis Tombados Isoladamente (Estadual/Federal)** | | |
| *   De 1 a 5 unidades | BI e/f 02 | **2** |
| *   De 6 a 10 unidades | BI e/f 04 | **4** |
| *   De 11 a 20 unidades | BI e/f 06 | **6** |
| *   Acima de 20 unidades | BI e/f 08 | **8** |
| **Bens Móveis Tombados Isoladamente (Estadual/Federal)** | | |
| *   De 1 a 20 unidades | BM e/f 01 | **1** |
| *   De 21 a 50 unidades | BM e/f 02 | **2** |
| *   Acima de 50 unidades | BM e/f 03 | **3** |
| **Núcleo Histórico Tombado (Municipal)** | | |
| *   De 20 a 2.000 unidades | NH mun | **3** |
| *   Acima de 2.000 unidades | NH mun | **4** |
| **Ações Municipais de Salvaguarda (Outras Pontuações)** | | |
| *   Educação Patrimonial Municipal (Projetos e atividades) | EP mun | **2** |
| *   Inventário de Proteção do Patrimônio Cultural elaborado | INV mun | **2** |
| *   Criação de Fundo Municipal de Preservação Cultural (**FUMPAC**) | FU mun | **3** |
| *   Existência de Planejamento e Política Municipal de Proteção | PCL mun | **4** |

---

## 🧮 Fórmulas e Modelagem de Pontuação (DN CONEP nº 01/2021)

A pontuação final do município é apurada pelo IEPHA-MG com base em 3 Quadros de Ação divididos em **8 Conjuntos Documentais** específicos, combinando pontuações fixas e proporcionais:

### QUADRO I — GESTÃO (Máximo: 7,0 pontos)
*   **Quadro IA: Política Municipal de Proteção (Atributo PCL) — Máx: 4,0 pontos**
    *   *Composição:* Lei municipal de patrimônio ativa; Conselho de Patrimônio em atividade (deliberativo, paritário); atuação do **SEMPAC** (Setor Municipal de Patrimônio); organização de acervos (pontos de memória, arquivos, bibliotecas); adesão a políticas estaduais, como o cadastro no programa **Invest Minas - Sustentabilidade de Patrimônios Culturais** (pontuação de `0,10 pts` verificada diretamente pela listagem oficial de cadastrados do IEPHA-MG, conforme Portaria nº 55/2023).
*   **Quadro IB: Investimentos e Fundo Municipal (Atributo FU) — Máx: 3,0 pontos**
    *   *Composição:* Criação e manutenção do **FUMPAC** (Fundo Municipal de Preservação); comprovação de **conta exclusiva** vinculada; repasses financeiros efetivos do caixa único e investimentos documentados em proteção/salvaguarda de bens protegidos e educação patrimonial.

### QUADRO II — PROTEÇÃO (Inventário Máx: 2,0 + Bens Proporcionais)
*   **Quadro IIA: Inventário Municipal (Atributo INV) — Máx: 2,0 pontos**
    *   *Composição:* Elaboração, execução e atualização do Plano de Inventário do Patrimônio Cultural (IPAC) do município.
*   **Quadro IIB: Processos de Tombamento de Bens Materiais**
    *   *Composição:* Dossiês de tombamento definitivo na esfera municipal (Núcleos Históricos `NH mun`, Conjuntos Urbanos/Paisagísticos `CP mun`, Bens Imóveis `BI mun` e Bens Móveis `BM mun`). *Pontuação proporcional.*
*   **Quadro IIC: Processos de Registro de Bens Imateriais (Atributo RI)**
    *   *Composição:* Processos de registro definitivo de patrimônios intangíveis locais com participação ativa dos detentores do bem. *Pontuação proporcional.*

### QUADRO III — SALVAGUARDA E PROMOÇÃO (Educação Máx: 2,0 + Relatórios Proporcionais)
*   **Quadro IIIA: Laudos Técnicos de Estado de Conservação**
    *   *Composição:* Monitoramento anual do estado físico dos bens materiais tombados sob competência municipal e propostas técnicas de intervenção. *Pontuação proporcional.*
*   **Quadro IIIB: Relatórios de Salvaguarda de Bens Imateriais**
    *   *Composição:* Relatórios anuais de execução dos planos de salvaguarda dos bens imateriais registrados na cidade. *Pontuação proporcional.*
*   **Quadro IIIC: Programas de Educação e Difusão (Atributo EP) — Máx: 2,0 pontos**
    *   *Composição:* Apresentação a cada 4 anos do **Plano de Ação de Educação para o Patrimônio e Difusão**. O município deve executar e comprovar no mínimo **8 ações anuais** (incluindo formação de servidores/conselheiros, difusão com escolas, comunidade, turistas e elaboração de material didático de suporte).

---

## 🔍 Como o Município Deve Auditar o Critério (Portaria IEPHA nº 34/2024 e nº 51/2025)

A Portaria regulamenta a apuração anual, a transmissão digital e os canais formais para contestação de pontos:

### Passo 1: Envio da Documentação via FTP
*   **Onde e Como Enviar:** A documentação dos Quadros I, II e III deve ser transmitida on-line via **protocolo FTP** no endereço **`ftp://200.198.49.202`**. O passo a passo completo de configuração de acesso está detalhado no **[Tutorial de Acesso FTP - IEPHA](https://www.mg.gov.br/sites/default/files/iepha/images/ICMS_2023/Orientacoes_Acesso_FTP_envio_quadros.pdf)**.
*   **⚠️ Calendário de Prazos (Portaria nº 51/2025):** 
    *   *Exercício 2027 (ano-base 2025) e subsequentes:* O envio deve ser realizado obrigatoriamente e exclusivamente por FTP no período de **20 de outubro a 20 de janeiro** do ano seguinte ao ano-base das ações. O envio físico via Correios foi descontinuado pela Portaria nº 51/2025.
    *   *Exercícios Anteriores (ano-base 2024 e retroativos):* A janela regular de envio da Portaria nº 34/2024 ocorria de **16 de outubro a 16 de janeiro**.

### Passo 2: Auditoria da Admissibilidade e Recurso de Envio
Até 30 dias após o fim das postagens, o IEPHA publica a lista de municípios com documentação recebida.
*   **Ação:** Se o nome do município ou de algum quadro enviado não constar na lista de admissibilidade, o prefeito ou procurador deve interpor recurso em até **10 dias corridos** via e-mail para **`icms@iepha.mg.gov.br`**, anexando o comprovante ou print de envio FTP (tamanho máximo de 3MB). A Diretoria de Promoção (DPR) tem 20 dias corridos para julgar.

### Passo 3: Auditoria da Pontuação Provisória e Impugnação GAM
Quando as Fichas de Análise forem disponibilizadas via FTP (no endereço **`ftp://200.198.51.131`**), o auditor municipal deve confrontar as penalidades e reduções de pontos aplicadas.
*   **⚠️ Prazo de Impugnação Provisória:** O município tem **10 dias corridos** (contados do primeiro dia útil seguinte à publicação) para contestar a pontuação provisória.
*   **Como Interpor:** Deve enviar e-mail exclusivo para a Gerência de Articulação com Municípios (GAM), respeitando a pasta setorial do recurso:
    *   Quadro IA: `icmsq1a@iepha.mg.gov.br`
    *   Quadro IB: `icmsq1b@iepha.mg.gov.br`
    *   Quadro IIA: `icmsq2a@iepha.mg.gov.br`
    *   Quadro IIB e IIIA: `icmsq2b-q3a@iepha.mg.gov.br`
    *   Quadro IIC e IIIB: `icmsq2c-q3b@iepha.mg.gov.br`
    *   Quadro IIIC: `icmsq3c@iepha.mg.gov.br`
*   **Assunto Obrigatório:** `NOME DO MUNICÍPIO - QUADRO e CONJUNTO DOCUMENTAL - CÓDIGO ALFANUMÉRICO` (extraído da Ficha de Análise).
*   *Nota:* Não é permitido anexar novos documentos nesta fase. A contestação deve se limitar a apontar erros de interpretação nos documentos já enviados no prazo regular.

### Passo 4: Recurso Final da Pontuação Definitiva via Sistema SEI
Se após a decisão da GAM a pontuação definitiva for publicada com erros:
*   **Prazo:** O município tem **15 dias corridos** após a publicação provisória para impugnar.
*   **Como Enviar:** Ofício dirigido à Presidência do IEPHA-MG, obrigatoriamente protocolado via **Sistema SEI** (através de peticionamento eletrônico de usuário externo). O Presidente do IEPHA profere a decisão final e encaminha as correções à Fundação João Pinheiro.

---

## 🛠️ Como o Município Pode Melhorar o Índice

1.  **Implantar o SEMPAC Efetivo:** Instituir por lei o Setor Municipal de Patrimônio Cultural ativo, organizando e disponibilizando os inventários físicos e digitais na prefeitura (pontua no Quadro IA).
2.  **Regularizar Repasses ao FUMPAC:** Fazer a transferência financeira real dos valores de ICMS arrecadados pelo critério de patrimônio de exercícios passados para a conta exclusiva do fundo e gastar em obras de restauro e promoção local (pontua no Quadro IB).
3.  **Realizar 8 Ações de Educação Patrimonial por Ano:** Seguir rigorosamente o Plano Quadrienal de Educação Patrimonial, garantindo a realização de no mínimo 8 ações no ano-base divididas entre servidores, comunidade, rede escolar e produção de cartilhas (pontua no Quadro IIIC).
4.  **Criar Tombamentos e Registros Definitivos:** Homologar processos definitivos em âmbito municipal e registrar bens imateriais (festividades locais, patrimônios culinários) com ampla documentação e participação da comunidade (Quadro IIB e IIC).

---
*Documento de estudo com base na Lei nº 18.030/2009, Deliberação Normativa CONEP nº 01/2021, Portaria IEPHA-MG nº 34/2024, Portaria nº 55/2023 e Portaria nº 51/2025. Mais informações e atualizações sobre o programa podem ser acessadas diretamente no site do **[Programa ICMS Patrimônio Cultural - IEPHA](https://www.mg.gov.br/iepha/pagina/programa-icms-patrimonio-cultural)**.*

---
title: Critério Recursos Hídricos
tags:
  - criterio-repasse
  - recursos-hidricos
  - energia
  - aneel
  - sef
date: 2026-07-01
weight: 0.25
---

# 💧 Critério Recursos Hídricos

O critério **Recursos Hídricos** distribui **0,25%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009).

> [!info] Compensação por Áreas Alagadas
> Este critério visa compensar financeiramente os municípios que tiveram porções de suas terras produtivas ou áreas urbanas alagadas para a construção de reservatórios de usinas hidrelétricas destinadas à geração de energia.

---

## 🧮 Fórmulas e Regras de Rateio (Art. 6º)

A distribuição da verba de Recursos Hídricos (0,25% do repasse aos municípios) ocorre de forma proporcional ao impacto do alagamento de terras pelas hidrelétricas situadas no estado, seguindo o rito de cálculo abaixo:

### Passo 1: Divisão do Valor Adicionado da Usina
Para cada usina hidrelétrica geradora de energia elétrica, apura-se o seu valor adicionado na operação de geração do ano anterior ($V_{\text{geração}}$), dividindo esse valor por dois:

$$V_{\text{rateio}} = \frac{V_{\text{geração}}}{2}$$

### Passo 2: Rateio entre Municípios com Áreas Alagadas (Excluindo Sede)
O montante $V_{\text{rateio}}$ é distribuído entre os municípios que possuem áreas alagadas pelo reservatório da usina e que **não são a sede física da usina**. A distribuição é estritamente proporcional à extensão da área do reservatório contida no território de cada município.
*   Os dados oficiais sobre as áreas dos reservatórios em cada município são obtidos da **ANEEL (Agência Nacional de Energia Elétrica)** e consolidados pela Secretaria de Estado de Fazenda (**SEF-MG**).

$$V_{i, u} = V_{\text{rateio}, u} \times \frac{\text{Área Alagada}_{i, u}}{\text{Área Alagada Total}_u}$$

Onde:
*   $V_{i, u}$ = Valor atribuído ao município $i$ em relação à usina $u$.
*   $\text{Área Alagada}_{i, u}$ = Área do reservatório da usina $u$ no município $i$.
*   $\text{Área Alagada Total}_u$ = Área total do reservatório da usina $u$ no Estado de Minas Gerais.

### Passo 3: Base de Cálculo Final do Município
A base de cálculo individual de participação do município no critério é o somatório dos valores de todas as usinas hidrelétricas ($u$) que o afetam:

$$B_i = \sum_{u} V_{i, u}$$

### Passo 4: Índice de Participação ($IP_{RH}$)
Por fim, o índice individual de participação do município no critério Recursos Hídricos ($IP_{RH, i}$) é obtido pela proporção de sua base de cálculo sobre a soma das bases de todos os municípios habilitados no critério:

$$IP_{RH, i} = \frac{B_i}{\sum_{j} B_j} \times 0,25\%$$

---

## 🚫 Regra de Exclusão (Art. 6º, Parágrafo Único)
Ficam excluídas do cálculo as áreas de reservatório que estejam dentro do território do **município sede da usina** cujo movimento econômico (Valor Adicionado) já tenha sido computado integralmente no cálculo do critério de participação no **VAF** (Art. 1º, inciso I). Essa regra evita a duplicidade de ganhos pelo mesmo ativo produtor.

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 6º|Art. 6º]] da Lei nº 18.030/2009.*

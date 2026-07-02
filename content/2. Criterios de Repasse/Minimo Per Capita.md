---
title: Critério Mínimo Per Capita
tags:
  - criterio-repasse
  - equidade-fiscal
  - fjp
  - legislacao
date: 2026-07-01
weight: 3.75
---

# 📈 Critério Mínimo Per Capita

O critério **Mínimo Per Capita** distribui **3,75%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009, atualizado pela Lei nº 24.431/2023).

> [!important] Piso de Repasse
> Este critério funciona como uma "rede de segurança" ou piso de proteção social e fiscal, garantindo que nenhum cidadão mineiro resida em um município que receba uma cota-parte de ICMS inferior a 50% da média per capita estadual.

---

## 🧮 Funcionamento do Cálculo (Art. 11)

A verba de 3,75% deste critério destina-se apenas aos municípios cujo índice consolidado de ICMS per capita (calculado considerando todos os critérios anteriores do Art. 1º, de I a XVII) seja inferior a **50% da média do Estado**.

O repasse individual é feito de forma proporcional ao **complemento necessário** para que o município atinja esse piso mínimo:

$$IP_{MPC, i} = \frac{Complemento_i}{\sum_{j} Complemento_j} \times 3,75\%$$

Onde os termos são modelados da seguinte forma:

### 1. Índice de ICMS Per Capita do Município ($ICMS\_PC_i$)
É a soma dos índices individuais de participação de cada município nos critérios de I a XVII dividida pela sua população ($Pop_i$):

$$ICMS\_PC_i = \frac{\sum_{k=1}^{17} IP_{k, i}}{Pop_i}$$

### 2. Média do Estado ($M_{\text{Estado}}$)
É o equivalente a dividir o índice total dos municípios (100% ou 1.0) pela população total do Estado de Minas Gerais ($Pop_{\text{Estado}}$):

$$M_{\text{Estado}} = \frac{100}{Pop_{\text{Estado}}}$$

### 3. Percentual Mínimo (Piso)
O piso per capita de repasse é fixado em 50% da média estadual:

$$\text{Piso} = 50\% \times M_{\text{Estado}}$$

### 4. Complemento Individual ($Complemento_i$)
Para municípios onde a receita acumulada estimada per capita ($ICMS\_PC_i$) é inferior ao Piso, calcula-se a diferença positiva:

$$Complemento_i = \left( \text{Piso} \times Pop_i \right) - \sum_{k=1}^{17} IP_{k, i}$$

Se o município já recebe acima do piso ($ICMS\_PC_i \ge \text{Piso}$), o complemento é zero ($Complemento_i = 0$).

---

## 🛡️ Cláusula de Contingência (Art. 11, Parágrafo Único)
Na hipótese de a distribuição dos demais critérios elevar a receita de todos os municípios de tal forma que nenhum atenda ao requisito de ficar abaixo do piso de 50% da média do Estado, os recursos desse critério (3,75%) serão transferidos e distribuídos integralmente pelo critério do **ICMS Solidário** (Art. 1º, inciso XVII).

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 11|Art. 11]] da Lei nº 18.030/2009.*

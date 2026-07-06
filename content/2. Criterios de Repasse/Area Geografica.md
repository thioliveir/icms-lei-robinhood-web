---
title: Área Geográfica
tags:
  - criterio-repasse
  - geografia
  - fjp
date: 2026-07-01
weight: 1.00
---

# 🗺️ Área Geográfica

O critério **Área Geográfica** distribui **1,00%** do ICMS pertencente aos municípios em Minas Gerais (conforme o Anexo I da Lei nº 18.030/2009).

---

## 🔍 O que é o Critério da Área Geográfica?

Este critério é puramente territorial e visa compensar os municípios que possuem grandes extensões territoriais terrestres. A lógica por trás deste critério é que municípios territorialmente maiores enfrentam custos elevados para manutenção de estradas vicinais, infraestrutura rural e deslocamento de serviços públicos (saúde, transporte escolar, etc.).

A lei define o critério como:
> *"II – área geográfica: relação percentual entre a área geográfica do município e a área total do Estado, informadas pela Fundação João Pinheiro – FJP"*

---

## 🧮 Fórmula de Cálculo ($IP_{AG}$)

O índice individual de participação de um município no critério Área Geográfica ($IP_{AG, i}$) é calculado da seguinte forma:

$$IP_{AG, i} = \frac{Area_i}{\sum_{j=1}^{853} Area_j} \times 1\%$$

Onde:
*   $Area_i$ = Área total do município $i$ em quilômetros quadrados ($km^2$), conforme base cartográfica da FJP.
*   $\sum_{j=1}^{853} Area_j$ = Soma das áreas de todos os 853 municípios de Minas Gerais (aproximadamente $586.783,33 \text{ km}^2$, conforme base consolidada da FJP).
*   Os dados de área oficial são atualizados e informados periodicamente pela **Fundação João Pinheiro (FJP)**.

### 📊 Exemplo Prático de Cálculo (Exercício 2026)

Tomando como exemplo o município de **Abadia dos Dourados** para o ano de 2026:
*   **Área oficial do município (FJP):** $883,17 \text{ km}^2$
*   **Área total somada do Estado (FJP):** $586.783,33 \text{ km}^2$

Aplica-se a fórmula:

$$IP_{AG} = \left( \frac{883,17 \text{ km}^2}{586.783,33 \text{ km}^2} \right) \times 1\%$$

$$IP_{AG} = 0,0015051043603 \times 1\%$$

Multiplicando por 100 para obter a taxa percentual e aplicando a precisão padrão da FJP (9 casas decimais):

$$IP_{AG} = \mathbf{0,150510436\%}$$

---

## 🔍 Como o Município Deve Auditar o Índice da Área Geográfica

O cálculo desse índice parece simples, mas exige que a prefeitura monitore com precisão os dados que a FJP insere na fórmula.

### ⚠️ A Armadilha da Área do IBGE
O erro mais frequente das prefeituras ao auditar este critério é utilizar o valor de área divulgado pelo **IBGE** (que, no exemplo de Abadia dos Dourados, é de $880,461 \text{ km}^2$). 
*   **A Razão:** A FJP possui uma diretoria própria de **Geografia e Cartografia** que revisa as divisas intermunicipais de Minas Gerais (leis de limites territoriais estaduais) de forma autônoma. O valor considerado no cálculo do ICMS é **exclusivamente o da FJP**, e não o do IBGE.
*   *Recomendação:* Baixe a planilha do critério *Área Geográfica* diretamente no **[Portal da Lei Robin Hood da FJP](https://robin-hood.fjp.mg.gov.br/extratos/anual)** e certifique-se de que a área considerada para o seu município corresponde ao mapeamento cartográfico estadual atualizado.

### Roteiro de Verificação da Divisa Municipal
1.  **Monitorar Projetos de Redefinição de Limites:** Acompanhar projetos na Assembleia Legislativa (ALMG) e na FJP de redefinição de limites territoriais que possam subtrair terras produtivas ou áreas urbanas do município.
2.  **Identificar Inconsistências de Mapeamento:** Caso o município identifique que distritos ou áreas limítrofes estão sendo catalogados erroneamente no território do município vizinho, deve apresentar uma **impugnação cartográfica** fundamentada junto à FJP, instruída por engenheiros ou agrimensores.

---

## 🛠️ Como o Município Pode Melhorar o Índice
Diferente de critérios como Educação ou Turismo, a área geográfica terrestre de um município é um dado estático. A única forma de "melhorar" ou proteger esse índice é:
*   **Defesa de Limites:** Garantir que litígios territoriais históricos ou novas demarcações de divisas com municípios vizinhos não diminuam a área oficial do seu município.
*   **Processos de Emancipação ou Fusão:** Embora raros atualmente, fusões de distritos ou incorporações de áreas expandem o território oficial e, proporcionalmente, aumentam o índice de participação do critério.

---

## 🔗 Relação com Outros Critérios
Este critério atua como um contrapeso direto ao critério de População e VAF, pois municípios muito extensos territorialmente localizados em regiões agrícolas ou de cerrado (como Unaí, Paracatu e Arinos) costumam ter um peso territorial expressivo, mesmo não tendo densidade populacional ou atividade industrial tão alta.

---
*Documento de estudo com base no [[Lei 18030-2009#Art. 1º|Art. 1º, II]] da Lei nº 18.030/2009.*

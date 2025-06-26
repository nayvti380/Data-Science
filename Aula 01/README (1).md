
# 📊 Aula de Data Science com Pandas – Análise de Fraude

Este repositório contém um notebook de introdução à análise de dados utilizando a biblioteca **Pandas**, com foco em práticas comuns de exploração de dados em projetos de **Data Science**.

Durante a aula, foram aplicadas técnicas básicas de manipulação de dados usando um **dataset real de detecção de fraudes**.

---

## 🧰 Bibliotecas Utilizadas

```python
import pandas as pd
import numpy as np
```

---

## 📍 Trabalhando com `pd.Series`

Criamos uma série com todas as siglas dos estados brasileiros:

```python
uf = ["AC", "AL", "AP", "AM", "BA", "CE",
      "DF", "ES", "GO", "MA", "MT", "MS",
      "MG", "PA", "PB", "PR", "PE", "PI",
      "RJ", "RN", "RS", "RO", "RR", "SC",
      "SP", "SE", "TO"]

uf = pd.Series(uf)
uf
```

---

## 📂 Leitura do Dataset

O arquivo utilizado foi:  
📄 `/content/Fraud Detection Dataset.csv`

```python
data_path = r"/content/Fraud Detection Dataset.csv"
df = pd.read_csv(data_path)
```

---

## 🔎 Análise Inicial dos Dados

A seguir, foram feitas verificações iniciais no dataset:

```python
df.tail()             # Visualiza as últimas linhas
df.sample(5)          # Visualiza uma amostra aleatória
df.shape              # Mostra o tamanho do DataFrame
df.info()             # Informações das colunas
df.isnull().sum()     # Verifica valores nulos
```

---

## 🧪 Amostragem de Linhas

- ✅ Primeiras 3 linhas:
```python
df.head(3)
```

- ✅ Últimas 8 linhas:
```python
df.tail(8)
```

- ✅ 10 linhas aleatórias:
```python
df.sample(10)
```

---

## 🎯 Objetivos da Aula

- 📌 Entender o que é uma `Series` e um `DataFrame` no Pandas.
- 📌 Aprender a importar e visualizar um dataset.
- 📌 Observar informações iniciais como número de linhas e colunas, tipos de dados e valores nulos.
- 📌 Realizar amostragens específicas e aleatórias.

---

## 💻 Requisitos

Certifique-se de ter o Python instalado com as bibliotecas abaixo:

```bash
pip install pandas numpy
```

---

## 👩‍🏫 Professor e Instituição

**Professor:** Walter  
**Escola:** Infinity School

---

## 👩‍💻 Ambiente Utilizado

A aula foi conduzida no **Google Colab**, um ambiente gratuito para notebooks Python na nuvem.

---

## 📎 Créditos

Material desenvolvido como parte da introdução prática à análise de dados com Python e Pandas, sob orientação do professor Walter, na **Infinity School**.

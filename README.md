# Avaliação A1 – Tecnologia e Desenvolvimento de Algoritmos (TDA)

Este repositório reúne todas as atividades desenvolvidas para a Avaliação A1 da disciplina **Tecnologia e Desenvolvimento de Algoritmos**.
Aqui estão organizados os códigos, explicações, exemplos, pseudocódigos e links dos notebooks no Google Colab.

---

## 🗂️ Estrutura do Repositório

```
Avaliação_A1_TDA/
├── README.md
├── LICENSE
│
├── 1_Estruturas_Condicionais/
│   └── verificacao_idade.py
│
├── 2_Estruturas_de_Repeticao/
│   └── pares_for_while.py
│
├── 3_Listas/
│   └── cadastro_alunos.py
│
└── 4_Dicionarios/
    └── cadastro_produtos.py
```

---

## 📎 Google Colab – Atividades

**Atividade 1 – Estruturas Condicionais**
🔗 [https://colab.research.google.com/drive/159wrnFaoe8ywcCt3N5wKIBn5BgjMy9XV?usp=sharing](https://colab.research.google.com/drive/159wrnFaoe8ywcCt3N5wKIBn5BgjMy9XV?usp=sharing)

**Atividade 2 – Estruturas de Repetição**
🔗 [https://colab.research.google.com/drive/1JItn_Mk4IU1KomvEpulE7j1nShRhKxxf?usp=sharing](https://colab.research.google.com/drive/1JItn_Mk4IU1KomvEpulE7j1nShRhKxxf?usp=sharing)

**Atividade 3 – Listas**
🔗 [https://colab.research.google.com/drive/1kDKsprc0MhhtiIqmk9N48BvxTVhOsV5a?usp=sharing](https://colab.research.google.com/drive/1kDKsprc0MhhtiIqmk9N48BvxTVhOsV5a?usp=sharing)

**Atividade 4 – Dicionários**
🔗 [https://colab.research.google.com/drive/1epRrHTMBV5ai90FpiGzzx4XXcr4PJ2bq?usp=sharing](https://colab.research.google.com/drive/1epRrHTMBV5ai90FpiGzzx4XXcr4PJ2bq?usp=sharing)

---

# 📝 Explicação, Pseudocódigo e Exemplos de Cada Atividade

---

# ✅ **1) Estruturas Condicionais – Verificação de Idade**

**Arquivo:** `1_Estruturas_Condicionais/verificacao_idade.py`

### 📌 O QUE O PROGRAMA FAZ?

Lê a idade do usuário e informa se sua entrada é:

* Permitida
* Permitida com responsável
* Proibida

### 🔎 **Pseudocódigo**

```
INICIO
  LER idade
  SE idade >= 18 ENTÃO
      ESCREVER "Entrada permitida! Você é maior de idade."
  SENÃO SE idade >= 16 ENTÃO
      ESCREVER "Entrada permitida somente com responsável."
  SENÃO
      ESCREVER "Entrada proibida. Você é menor de 16 anos."
  FIMSE
FIM
```

### 🧪 **Exemplo de Entrada e Saída**

**Entrada:**

```
idade = 20
```

**Saída:**

```
Entrada permitida! Você é maior de idade.
```

---

**Entrada:**

```
idade = 16
```

**Saída:**

```
Entrada permitida somente com responsável.
```

---

**Entrada:**

```
idade = 14
```

**Saída:**

```
Entrada proibida. Você é menor de 16 anos.
```

---

# ✅ **2) Estruturas de Repetição – Exibir Números Pares**

**Arquivo:** `2_Estruturas_de_Repeticao/pares_for_while.py`

### 📌 O QUE O PROGRAMA FAZ?

Mostra todos os números pares de **1 a 100**, usando:

* Um laço **for**
* Um laço **while**

### 🔎 **Pseudocódigo Correto**

```
INICIO
  ESCREVER "Números pares usando FOR"
  PARA num DE 1 ATÉ 100 PASSO 1 FAÇA
      SE num % 2 == 0 ENTÃO
          ESCREVER num
      FIMSE
  FIMPARA

  ESCREVER "Números pares usando WHILE"
  num ← 1
  ENQUANTO num <= 100 FAÇA
      SE num % 2 == 0 ENTÃO
          ESCREVER num
      FIMSE
      num ← num + 1
  FIMENQUANTO
FIM
```

### 🧪 **Exemplo de Saída (abreviado)**

```
Números pares usando FOR:
2
4
6
...
100

Números pares usando WHILE:
2
4
6
...
100
```

O comportamento é idêntico nos dois laços.

---

# ✅ **3) Listas – Cadastro de Alunos**

**Arquivo:** `3_Listas/cadastro_alunos.py`

### 📌 O QUE O PROGRAMA FAZ?

* Cria uma lista vazia
* Lê 3 nomes digitados pelo usuário
* Armazena todos na lista
* Exibe o resultado final

### 🔎 **Pseudocódigo**

```
INICIO
  CRIAR lista_alunos VAZIA
  
  PARA i DE 1 ATÉ 3 FAÇA
      LER nome
      ADICIONAR nome NA lista_alunos
  FIMPARA
  
  ESCREVER lista_alunos
FIM
```

### 🧪 **Exemplo de Entrada**

```
João
Maria
Carlos
```

### 🧪 **Saída**

```
['João', 'Maria', 'Carlos']
```

---

# ✅ **4) Dicionários – Cadastro de Produtos**

**Arquivo:** `4_Dicionarios/cadastro_produtos.py`

### 📌 O QUE O PROGRAMA FAZ?

* Cria um dicionário
* Lê nome, preço e quantidade do produto
* Armazena os valores no dicionário
* Exibe o produto completo

### 🔎 **Pseudocódigo**

```
INICIO
  CRIAR produtos COMO DICIONARIO VAZIO

  ESCREVER "Cadastro de produtos (digite 'sair' para encerrar')"

  ENQUANTO VERDADEIRO FAÇA
      LER nome

      SE nome = "sair" ENTÃO
          PARAR O LOOP
      FIMSE

      LER preco
      LER quantidade

      produtos[nome] ← DICIONARIO {
          "preco": preco,
          "quantidade": quantidade
      }
  FIMENQUANTO

  ESCREVER "Produtos cadastrados:"

  PARA CADA nome, dados EM produtos FAÇA
      ESCREVER nome, dados["preco"], dados["quantidade"]
  FIMPARA
FIM

```

### 🧪 **Exemplo de Entrada**

```
Nome: Mouse Gamer
Preço: 129.90
Quantidade: 4
```

### 🧪 **Saída**

```
{'nome': 'Mouse Gamer', 'preco': 129.9, 'quantidade': 4}
```

---

# ✔️ O que este trabalho demonstra

* Domínio de condicionais, repetições, listas e dicionários
* Capacidade de resolver problemas com lógica
* Organização do repositório com boa estrutura
* Pseudocódigo + código funcionando + exemplos
* Uso de Google Colab para testes e documentação

---

# 📄 Licença

Este projeto está sob a licença **MIT**.

---

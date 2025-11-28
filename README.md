# 📘 Avaliação A1 – Técnicas de Desenvolvimento de Algoritmos

Este repositório contém as quatro atividades avaliativas da disciplina **TDA – Técnicas de Desenvolvimento de Algoritmos**, trabalhando conceitos essenciais de lógica de programação: **estruturas condicionais**, **laços de repetição**, **listas** e **dicionários**.

Cada atividade possui:
✔ Código Python comentado
✔ Pseudocódigo correspondente
✔ Explicação do que o programa faz
✔ Exemplos de entrada e saída
✔ Link para execução no Google Colab

---

## 🗂️ Estrutura do Repositório

```
Avaliação_A1_TDA/
├── README.md
│
├── Estruturas_Condicionais/
│   └── verificacao_idade.py
│
├── Estruturas_de_Repeticao/
│   └── pares_for_while.py
│
├── Listas/
│   └── cadastro_alunos.py
│
└── Dicionarios/
    └── cadastro_produtos.py
```

---

# 🧩 **Atividade 1 – Estruturas Condicionais**

🔗 **Google Colab:**
[https://colab.research.google.com/drive/159wrnFaoe8ywcCt3N5wKIBn5BgjMy9XV?usp=sharing](https://colab.research.google.com/drive/159wrnFaoe8ywcCt3N5wKIBn5BgjMy9XV?usp=sharing)

### 📌 O que o programa faz?

Lê a idade do usuário e determina se a entrada é permitida, permitida com responsável ou proibida.

### ▶️ Exemplo de entrada:

```
17
```

### 🟢 Exemplo de saída:

```
Entrada permitida somente com responsável.
```

### 📎 Pseudocódigo

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

---

# 🔁 **Atividade 2 – Estruturas de Repetição**

🔗 **Google Colab:**
[https://colab.research.google.com/drive/1JItn_Mk4IU1KomvEpulE7j1nShRhKxxf?usp=sharing](https://colab.research.google.com/drive/1JItn_Mk4IU1KomvEpulE7j1nShRhKxxf?usp=sharing)

### 📌 O que o programa faz?

Exibe todos os números pares entre **1 e 100**, usando FOR e WHILE.

### ▶️ Exemplo de saída (trecho):

```
2
4
6
...
100
```

### 📎 Pseudocódigo (FOR)

```
INICIO
  PARA num DE 1 ATÉ 100 FAÇA
      SE num % 2 = 0 ENTÃO
          ESCREVER num
      FIMSE
  FIMPARA
FIM
```

### 📎 Pseudocódigo (WHILE)

```
INICIO
  num ← 1

  ENQUANTO num <= 100 FAÇA
      SE num % 2 = 0 ENTÃO
          ESCREVER num
      FIMSE
      
      num ← num + 1
  FIMENQUANTO
FIM
```

---

# 📝 **Atividade 3 – Listas**

🔗 **Google Colab:**
[https://colab.research.google.com/drive/1kDKsprc0MhhtiIqmk9N48BvxTVhOsV5a?usp=sharing](https://colab.research.google.com/drive/1kDKsprc0MhhtiIqmk9N48BvxTVhOsV5a?usp=sharing)

### 📌 O que o programa faz?

Cadastra nomes de alunos em uma lista e depois exibe todos os cadastrados.

### ▶️ Exemplo de entrada:

```
João
Maria
sair
```

### 🟢 Exemplo de saída:

```
Alunos cadastrados:
João
Maria
```

### 📎 Pseudocódigo

```
INICIO
  CRIAR lista_alunos COMO LISTA VAZIA
  
  REPETIR
      LER nome
      
      SE nome = "sair" ENTÃO
          PARAR
      FIMSE
      
      ADICIONAR nome NA lista_alunos
  ATÉ QUE nome = "sair"

  PARA CADA aluno EM lista_alunos FAÇA
      ESCREVER aluno
  FIMPARA
FIM
```

---

# 🛒 **Atividade 4 – Dicionários**

🔗 **Google Colab:**
[https://colab.research.google.com/drive/1epRrHTMBV5ai90FpiGzzx4XXcr4PJ2bq?usp=sharing](https://colab.research.google.com/drive/1epRrHTMBV5ai90FpiGzzx4XXcr4PJ2bq?usp=sharing)

### 📌 O que o programa faz?

Cadastra produtos utilizando dicionários. Cada produto possui nome, preço e quantidade.

### ▶️ Exemplo de entrada:

```
Arroz
12.50
3
sair
```

### 🟢 Exemplo de saída:

```
Arroz - R$ 12.50 - Quantidade: 3
```

### 📎 Pseudocódigo

```
INICIO
  CRIAR produtos COMO DICIONARIO
  
  REPETIR
      LER nome
      
      SE nome = "sair" ENTÃO
          PARAR
      FIMSE
      
      LER preco
      LER quantidade
      
      produtos[nome] ← { "preco": preco, "quantidade": quantidade }
  ATÉ QUE nome = "sair"

  PARA CADA item EM produtos FAÇA
      ESCREVER nome, preco, quantidade
  FIMPARA
FIM
```

---

# 📄 Licença – MIT License

```
MIT License

Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

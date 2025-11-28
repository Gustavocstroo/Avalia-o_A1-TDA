# 📘 Avaliação A1 — Técnicas de Desenvolvimento de Algoritmos

Este repositório contém quatro programas desenvolvidos em Python, cada um representando diferentes estruturas fundamentais da lógica de programação: **estruturas condicionais**, **estruturas de repetição (for e while)**, **listas** e **dicionários**.

Além do código-fonte, este README inclui **pseudocódigo** para facilitar a compreensão dos algoritmos utilizados.

---

## 🗂️ Estrutura do Repositório

```
Avaliação_A1_TDA/
├── README.md
├── LICENSE
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

# 📂 Detalhamento dos Programas

---

## ✅ **1. Estruturas Condicionais – verificacao_idade.py**

### 📌 **O que o programa faz**

O programa solicita a idade do usuário e utiliza **estrutura condicional (if/elif/else)** para determinar se a pessoa é:

* Menor de idade
* Maior de idade
* Idoso (≥ 60 anos)

### 🧠 **Pseudocódigo**

```
INÍCIO
    LER idade
    SE idade < 18 ENTÃO
        ESCREVER "Menor de idade"
    SENÃO SE idade >= 60 ENTÃO
        ESCREVER "Idoso"
    SENÃO
        ESCREVER "Maior de idade"
FIM
```

---

## ✅ **2. Estruturas de Repetição – pares_for_while.py**

### 📌 **O que o programa faz**

Este programa exibe **todos os números pares de 1 a 100**, usando:

* Um **laço FOR**
* Um **laço WHILE**

O objetivo é demonstrar a aplicação prática das duas estruturas de repetição.

---

### 🧠 **Pseudocódigo (FOR)**

```
INÍCIO
    PARA num DE 1 ATÉ 100 FAÇA
        SE num MOD 2 == 0 ENTÃO
            ESCREVER num
        FIMSE
    FIMPARA
FIM
```

### 🧠 **Pseudocódigo (WHILE)**

```
INÍCIO
    num ← 1
    ENQUANTO num <= 100 FAÇA
        SE num MOD 2 == 0 ENTÃO
            ESCREVER num
        FIMSE
        num ← num + 1
    FIMENQUANTO
FIM
```

---

## ✅ **3. Listas – cadastro_alunos.py**

### 📌 **O que o programa faz**

Este programa permite cadastrar nomes de alunos dentro de uma **lista**.
Ele solicita repetidamente um nome até que o usuário digite `"sair"`.

Ao final, exibe:

* Quantos alunos foram cadastrados
* A lista completa dos alunos

### 🧠 **Pseudocódigo**

```
INÍCIO
    CRIAR lista_alunos VAZIA
    REPETIR
        LER nome
        SE nome != "sair" ENTÃO
            ADICIONAR nome À lista_alunos
        FIMSE
    ATÉ nome == "sair"
    ESCREVER quantidade de alunos
    ESCREVER lista de alunos
FIM
```

---

## ✅ **4. Dicionários – cadastro_produtos.py**

### 📌 **O que o programa faz**

O programa permite cadastrar produtos com:

* Nome
* Preço

Cada produto é salvo em um **dicionário**, e vários dicionários são armazenados em uma lista.

Ao final, o programa exibe todos os produtos cadastrados.

### 🧠 **Pseudocódigo**

```
INÍCIO
    CRIAR lista_produtos VAZIA
    REPETIR
        LER nome_produto
        SE nome_produto != "sair" ENTÃO
            LER preco
            CRIAR dicionario_produto
            dicionario_produto["nome"] ← nome_produto
            dicionario_produto["preco"] ← preco
            ADICIONAR dicionario_produto À lista_produtos
        FIMSE
    ATÉ nome_produto == "sair"
    
    PARA cada produto EM lista_produtos FAÇA
        ESCREVER nome e preço do produto
    FIMPARA
FIM
```

---

# 📄 Licença

Este projeto utiliza a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---


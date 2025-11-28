# Avaliação A1 – Tecnologia e Desenvolvimento de Algoritmos (TDA)

Este repositório reúne todas as atividades desenvolvidas para a Avaliação A1 da disciplina **Tecnologia e Desenvolvimento de Algoritmos**.  
Aqui estão organizados os códigos, pseudocódigos e notebooks utilizados para resolver cada atividade.

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

## 📎 Google Colab – Atividades

Cada atividade também foi desenvolvida no Google Colab para facilitar testes e organização:

**Atividade 1 – Operações e Estruturas Básicas**  
🔗 https://colab.research.google.com/drive/159wrnFaoe8ywcCt3N5wKIBn5BgjMy9XV?usp=sharing  

**Atividade 2 – Estruturas Condicionais**  
🔗 https://colab.research.google.com/drive/1JItn_Mk4IU1KomvEpulE7j1nShRhKxxf?usp=sharing  

**Atividade 3 – Estruturas de Repetição**  
🔗 https://colab.research.google.com/drive/1kDKsprc0MhhtiIqmk9N48BvxTVhOsV5a?usp=sharing  

**Atividade 4 – Funções**  
🔗 https://colab.research.google.com/drive/1epRrHTMBV5ai90FpiGzzx4XXcr4PJ2bq?usp=sharing  

---

## 📝 Pseudocódigos das Atividades

### **1) Estruturas Condicionais – verificação de idade**

**Arquivo:** `Estruturas_Condicionais/verificacao_idade.py`

**Pseudocódigo:**
```
INICIO
  LER idade
  SE idade >= 18 ENTÃO
      ESCREVE "Entrada permitida! Você é maior de idade."
  SENÃO SE idade >= 16 ENTÃO
      ESCREVE "Entrada permitida somente com responsável."
  SENÃO
      ESCREVE "Entrada proibida. Você é menor de 16 anos."
  FIMSE
FIM
```

---

### **2) Estruturas de Repetição – números pares**

**Arquivo:** `Estruturas_de_Repeticao/pares_for_while.py`

**Pseudocódigo:**
```
INICIO
  PARA numero DE 0 ATÉ 20 PASSO 2 FAÇA
      ESCREVE numero
  FIMPARA
  
  numero ← 0
  ENQUANTO numero <= 20 FAÇA
      ESCREVE numero
      numero ← numero + 2
  FIMENQUANTO
FIM
```

---

### **3) Listas – cadastro de alunos**

**Arquivo:** `Listas/cadastro_alunos.py`

**Pseudocódigo:**
```
INICIO
  CRIAR lista_alunos VAZIA
  
  PARA i DE 1 ATÉ 3 FAÇA
      LER nome
      ADICIONAR nome NA lista_alunos
  FIMPARA
  
  ESCREVE lista_alunos
FIM
```

---

### **4) Dicionários – cadastro de produtos**

**Arquivo:** `Dicionarios/cadastro_produtos.py`

**Pseudocódigo:**
```
INICIO
  CRIAR produto COMO DICIONARIO
  
  LER nome
  LER preço
  LER quantidade
  
  produto["nome"] ← nome
  produto["preco"] ← preço
  produto["quantidade"] ← quantidade
  
  ESCREVE produto
FIM
```
---

## 📄 Licença
Este projeto está sob a licença **MIT**.

---

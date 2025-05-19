# 📦 API de Produtos com Spring Boot

Esta é uma API REST simples para gerenciamento de produtos desenvolvida com **Spring Boot**. O projeto foi criado durante um curso de introdução ao Spring Boot e tem como objetivo o aprendizado de conceitos fundamentais do framework.

---

## 🚀 Funcionalidades

A API permite realizar operações básicas de CRUD:

- **Criar** um novo produto (`POST /produtos`)
- **Buscar** um produto por ID (`GET /produtos/{id}`)
- **Atualizar** um produto existente (`PUT /produtos/{id}`)
- **Deletar** um produto (`DELETE /produtos/{id}`)

---

## 🛠 Tecnologias e Conceitos Aprendidos

Durante o desenvolvimento da API, foram estudados e aplicados os seguintes tópicos:

- 📦 **Spring Boot**: configuração básica, estrutura de projetos, criação de controllers e endpoints REST.
- 💾 **Banco de dados em memória H2**: uso inicial com persistência temporária para testes e desenvolvimento.
- 📚 **JPA (Java Persistence API)**: persistência de dados com o Spring Data.
- 🧠 **Injeção de dependência**: uso de construtores para injetar repositórios (`ProdutoRepository`).
- 🧰 **Lombok**: geração automática de getters, setters e construtores para simplificar o código (caso utilizado).
- 🧪 **Testes com Postman**: simulação de chamadas HTTP para testar os endpoints da API.

---

## 💡 Exemplos de Uso (via Postman)

### ▶️ Criar um produto

**POST** `http://localhost:8080/produtos`

```json
{
  "nome": "Notebook",
  "preco": 3500.00
}
````

---

### 🔍 Buscar um produto por ID

**GET** `http://localhost:8080/produtos/{id}`

---

### 🔁 Atualizar um produto

**PUT** `http://localhost:8080/produtos/{id}`

```json
{
  "nome": "Notebook Gamer",
  "preco": 4500.00
}
```

---

### 🗑️ Deletar um produto

**DELETE** `http://localhost:8080/produtos/{id}`

---

## 📌 Observações

* O banco de dados **H2** é reiniciado toda vez que a aplicação é finalizada, pois é um banco em memória.
* Os testes foram realizados utilizando o **Postman**, garantindo o funcionamento dos endpoints.



---

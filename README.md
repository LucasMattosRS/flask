# Painel de Vendas - StyleSync (API e Web App)

![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

Este repositório contém o código-fonte de uma API RESTful e uma aplicação web simples desenvolvida em Flask para gerenciamento de produtos e vendas. O projeto foi construído de forma incremental, seguindo as melhores práticas de desenvolvimento, como a separação de responsabilidades, validação de dados e autenticação segura.

## 📜 Sobre o Projeto

O "Painel de Vendas StyleSync" simula o back-end e uma interface de administração para uma startup de e-commerce fictícia. O objetivo é fornecer uma base sólida e escalável para gerenciar as principais entidades do negócio: produtos, usuários e vendas.

A aplicação foi desenvolvida com uma arquitetura que utiliza o padrão *Application Factory* e *Blueprints* para garantir a modularidade e facilitar a manutenção e os testes.

## ✨ Funcionalidades Principais

* **API RESTful Completa:** Endpoints para todas as operações CRUD (Criar, Ler, Atualizar, Deletar) de produtos.
* **Autenticação via JWT:** Sistema de login que gera um JSON Web Token para proteger rotas administrativas.
* **Upload de Dados em Massa:** Funcionalidade para importar registros de vendas através do upload de arquivos `.csv`.
* **Validação de Dados:** Uso da biblioteca Pydantic para validar a estrutura e os tipos de dados em todas as requisições de entrada.
* **Interface Web Simples:** Páginas HTML renderizadas pelo Flask (usando Jinja2) e estilizadas com Bootstrap para interagir com as funcionalidades do back-end.
* **Introdução a Testes:** Inclui um exemplo de teste unitário utilizando Pytest.

## 🛠️ Tecnologias Utilizadas

* **Back-end:**
    * **Python 3**
    * **Flask:** Microframework web para a construção da API e da aplicação.
    * **MongoDB:** Banco de dados NoSQL para persistência dos dados.
    * **PyMongo:** Driver oficial para conectar a aplicação Python ao MongoDB.
    * **Pydantic:** Para validação e modelagem de dados.
    * **PyJWT:** Para geração e validação de JSON Web Tokens.
* **Front-end:**
    * **HTML5** com **Jinja2 Templates**
    * **Bootstrap 5:** Para estilização e responsividade das páginas.
* **Testes:**
    * **Pytest:** Framework para testes unitários.

## 🌐 Interface Web

O projeto também serve uma interface web simples, construída com Flask Templates e Bootstrap, que permite interagir com a API. As páginas incluem:
* Página de Login (`/login`)
* Dashboard principal (`/dashboard`)
* Lista de Produtos (`/produtos`)
* Formulário para adicionar produtos (`/produtos/novo`)
* Formulário para upload de vendas (`/vendas/upload`)



Esta aplicação é uma base sólida que pode ser expandida. Algumas melhorias futuras planejadas incluem:
* **Containerização com Docker:** Facilitar o deploy e a portabilidade da aplicação.
* **Pipeline de CI/CD:** Automatizar os testes e o deploy com ferramentas como GitHub Actions.
* **Cache com Redis:** Melhorar a performance das rotas de leitura mais acessadas.
* **Sistema de Permissões (RBAC):** Criar diferentes níveis de acesso para os usuários (ex: admin, vendedor).


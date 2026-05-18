# 🗺️ API de Estados e Cidades do Brasil

API REST desenvolvida com Node.js e Express para consulta de dados geográficos dos estados e cidades brasileiras, com módulo dedicado para filtragem e manipulação dos dados em JSON.

**Autora:** [Daniele Silva Santos](https://www.linkedin.com/in/danielesilvasantos/) | **Versão:** 1.0 | **Data:** 01/04/2026

---

## 📋 Conceitos Aplicados

- **Express.js:** Criação de servidor HTTP e definição de rotas com parâmetros dinâmicos
- **CORS:** Configuração de permissões de acesso externo à API
- **Módulos:** Separação de responsabilidades entre `app.js` (rotas) e `functions.js` (lógica)
- **Manipulação de Arrays:** Uso de `.forEach()`, `.push()` e `.map()` para construção de coleções dinâmicas
- **Tratamento de Strings:** `.toUpperCase()` para buscas case-insensitive
- **Códigos HTTP:** Retorno semântico de status `200` e `404` conforme resultado da operação
- **Parâmetros de Rota:** Captura de dados dinâmicos via `request.params`
- **JSON Dinâmico:** Construção de objetos de resposta personalizados por endpoint

---

## 💻 Endpoints Disponíveis

| Método | Rota | Descrição |
|--------|------|-----------|
| GET | `/v1/senai/estados` | Lista as siglas de todos os estados e quantidade total |
| GET | `/v1/senai/dados/estado/:uf` | Retorna nome, capital e região de um estado pela sigla |
| GET | `/v1/senai/capital/estado/:uf` | Retorna os dados da capital de um estado pela sigla |
| GET | `/v1/senai/estados/regiao/:regiao` | Retorna todos os estados de uma região |
| GET | `/v1/senai/estados/capital/brasil` | Retorna os estados que já foram capital do Brasil |
| GET | `/v1/senai/estados/cidade/:uf` | Retorna todas as cidades de um estado e quantidade total |
| GET | `/v1/senai/help` | Retorna a documentação completa dos endpoints |

---

## 📂 Estrutura de Arquivos
```text
exercicio_06/
├── app.js                  # Servidor Express e definição das rotas
├── package.json
└── modulo/
    ├── functions.js        # Lógica de filtragem e funções exportadas
    └── estados_cidades.js  # Base de dados em JSON
└── front-end/
    ├── index.html        # Lógica do Web Site
```

---

## 🚀 Como Executar Localmente

**Pré-requisito:** Node.js instalado
```bash
# Instalar dependências
npm install

# Iniciar a API
node app.js
```

A API ficará disponível em: `http://localhost:8080`

---

## 🛠️ Tecnologias Utilizadas

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![CORS](https://img.shields.io/badge/CORS-enabled-blue?style=flat)

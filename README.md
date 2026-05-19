# 📋 TAP — Termo de Abertura do Projeto

## Objetivo
API REST desenvolvida para consulta de dados geográficos do Brasil,
retornando informações sobre estados, capitais, regiões e municípios.

---

## Tecnologias Utilizadas
- **Node.js** — ambiente de execução
- **Express** — framework HTTP para criação da API
- **CORS** — controle de permissões de acesso

---

## Endpoints Disponíveis
| Método | Rota | Descrição |
|--------|------|-----------|
| GET | `/v1/senai/estados` | Lista todos os estados |
| GET | `/v1/senai/dados/estado/:uf` | Dados de um estado pela sigla |
| GET | `/v1/senai/capital/estado/:uf` | Capital do estado pela sigla |
| GET | `/v1/senai/estados/regiao/:regiao` | Estados por região |
| GET | `/v1/senai/estados/capital/brasil` | Estados que foram capital do Brasil |
| GET | `/v1/senai/estados/cidade/:uf` | Cidades de um estado pela sigla |

---

## Como Executar Localmente
```bash
# Instalar dependências
npm install

# Iniciar a API
node app.js
```
A API ficará disponível em `http://localhost:8080`

---

## Autora
**Daniele Silva Santos** — SENAI — 2026

---

## Estimativa de Esforço e Custo

| Item | Valor |
|------|-------|
| Total de horas estimadas | 29h |
| Perfil | Desenvolvedor(a) Júnior |
| Valor hora | R$ 30,00 |
| **Custo total estimado** | **R$ 870,00** |

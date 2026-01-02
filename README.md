\# m3invest — PoC de Finanças Domésticas com Assistente LLM



Prova de conceito de um serviço onde o usuário autentica (login/senha) e registra:

\- renda, despesas, dívidas, metas/desejos

\- categorias opcionais (rol pré-definido + customizáveis)

\- persistência local (SQLite) para o PoC

\- cache/sessão em memória (evolui para Redis se necessário)



\## Stack (PoC)

\- Backend: FastAPI

\- Persistência: SQLite (SQLAlchemy + Alembic)

\- Auth: hash de senha (bcrypt) + JWT

\- Qualidade: Ruff + Pytest + pre-commit

\- CI: GitHub Actions



\## Rodar em desenvolvimento

1\) Criar ambiente:

```bash

conda env create -f environment.yml

conda activate m3invest




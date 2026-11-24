# API de chamados

**Nome completo:** Vitória Cavalcante Souza

## Objetivo

Criar a estrutura inicial de uma API de chamados de suporte com Flask. Nesta
etapa, a API disponibiliza apenas uma rota inicial de confirmação; não inclui
cadastro de chamados nem banco de dados.

## Instalação

Com o [uv](https://docs.astral.sh/uv/) instalado, sincronize o ambiente e as
dependências do projeto:

```bash
uv sync --locked
```

## Como executar

Na raiz do projeto, inicie a aplicação:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Rota inicial

Acesse `http://localhost:5000/` pelo navegador ou envie uma requisição:

```bash
curl -i http://localhost:5000/
```

A rota `GET /` deve responder com status `200`, `Content-Type:
application/json` e o seguinte corpo:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```

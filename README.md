# Configuração testada em Docker-compose

Escolha uma das versões e crie na pasta o arquivo `.env` conforme o exemplo `.env_example` .

## n8n-start

  + Esta versão não esta configurada para salvar os dados em disco, salva apenas em `volumes` `docker`. Cuidado ao remover os volumes para não perder os dados salvos.

## n8n-postgres

  + Esta versão esta configurada com volumes em persistencia da pasta `data`.

## n8n-postgres-worker <i>(RECOMENDADO !!!)</i>

  + Esta versão esta configurada com volumes em persistencia da pasta `data`.

  + `n8n-postgres-worker` -> Recomendado usar esta versão que contem `REDIS`,  `WORKERS` e banco de dados `POSTGRESQL`.

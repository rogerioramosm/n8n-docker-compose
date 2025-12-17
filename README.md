# Configuração testada em Docker-compose

## Contem 3 pastas:

### n8n-start

  + Esta versão não esta configurada para salvar os dados em disco, salva apenas em `volumes` `docker`. Cuidado ao remover os volumes para não perder os dados salvos.

### n8n-postgres

  + Esta versão esta configurada com volumes em persistencia da pasta `data`.

### n8n-postgres-worker

  + Esta versão esta configurada com volumes em persistencia da pasta `data`.

  + `n8n-postgres-worker` -> Recomendado usar esta versão que contem `REDIS`,  `WORKERS` e banco de dados `POSTGRESQL`.

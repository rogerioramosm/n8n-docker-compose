# Configuração testada em Docker-compose

Escolha uma das versões e crie na pasta o arquivo `.env` conforme o exemplo `.env_example` .

## Configuração no Linux

Execute as permissões do diretório de volumes antes de iniciar o `docker-compose` .

  + No `Windows` esta configuração não é necessária!

```bash

  # pasta /data é onde os volumes serão montados
  sudo chown -R 1000:1000 /data

  sudo chmod -R 755 data/

```

## n8n-start

  + Esta versão não esta configurada para salvar os dados em disco, salva apenas em `volumes` `docker`. Cuidado ao remover os volumes para não perder os dados salvos.

## n8n-postgres

  + Esta versão esta configurada com volumes em persistencia da pasta `data`.

## n8n-postgres-worker <i>(RECOMENDADO !!!)</i>

  + Esta versão esta configurada com volumes em persistencia da pasta `data`.

  + `n8n-postgres-worker` -> Recomendado usar esta versão que contem `REDIS`,  `WORKERS` e banco de dados `POSTGRESQL`.

## Inicialização

```bash
  # Linux
  sudo docker-compose up --build --force-recreate -d

  # Windows
  docker-compose up --build --force-recreate -d

  # Se na primeira tentativa gerar erro, pause e inicie novamente
  docker-compose stop
  docker-compose up --build --force-recreate -d
```

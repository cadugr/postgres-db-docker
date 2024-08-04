# PostgreSQL Docker Container Setup

Este repositório contém instruções para configurar e executar um banco de dados PostgreSQL dentro de um container Docker, conforme solicitado no desafio do módulo de Docker do curso devopspro.  Siga estes passos para colocar seu container PostgreSQL em funcionamento.

## Pré-requisitos

- [Docker](https://www.docker.com/get-started) instalado na sua máquina
- Conhecimento básico de operações de linha de comando

## Para criar o banco de dados:

Abra seu terminal e execute o seguinte comando:

```bash
docker container run -d -p 5432:5432 -e POSTGRES_DB="curso_docker" -e POSTGRES_USER="docker_usr" -e POSTGRES_PASSWORD="docker_pwd" postgres
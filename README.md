# Sentry 
## O que é sentry
O Sentry é uma cros-plataforma de monitoramento de aplicativos, com foco no relatório de erros.
Sentry é fundamentalmente um serviço que ajuda a monitorar e corrigir falhas em tempo real. O servidor está em Python, mas contém uma API completa para enviar eventos de qualquer liguagem de programação, em qualquer aplicativo.

## Como usar essa ferramenta?

Primeiramente inicie uma sessao do bash com o container do sentry:
```sh
    docker-compose run sentry bash
```

Depois execute o comando abaixo para criar o banco de dados e as tabelas:
```sh
    sentry update
```
Apos finalizar a criação das tabelas execulte o compose:
```sh
    docker-compose up
```
ou
```sh
    docker-compose up -d
```
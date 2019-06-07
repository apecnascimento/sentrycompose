# Sentry 
## O que é sentry
O Sentry é uma ferramenta cros-plataforma de monitoramento de aplicativos, com foco no relatório de erros.
Sentry é fundamentalmente um serviço que ajuda a monitorar e corrigir falhas em tempo real. O servidor está em Python, mas contém uma API completa para enviar eventos de qualquer liguagem de programação, em qualquer aplicativo.

## Como usar essa ferramenta?

Primeiramente crie uma chave de segurança do sentry. Essa chave é usada para encriptar informações confidenciais no sentry:
```sh
    docker-compose run --rm sentry sentry config generate-secret-key
```
Adicione a chave dse seguranção gerada pelo sentry na variavel de anbiente SENTRY_SECRET_KEY.

Depois execute o comando abaixo para criar o banco de dados e as tabelas:
```sh
     docker-compose run --rm sentry sentry upgrade
```
Apos finalizar a criação das tabelas execulte o compose:
```sh
    docker-compose up
```
ou
```sh
    docker-compose up -d
```

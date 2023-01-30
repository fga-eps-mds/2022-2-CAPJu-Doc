# Manual de instalação

# 1. Introdução

Essa sessão tem como objetivo orientar o passos a passos para rodar esse projeto em sua máquina local

# 2. Requisitos mínimos 

## Hardware

- 8 GB de RAM
- Sistema operacional Linux/MacOS - (Intel)

## Software

- Node vesão 14 - Recomendo o uso de [nvm](https://github.com/nvm-sh/nvm)
- Biblioteca [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/#mac-stable)
- [GIT](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Postgres 14 ou superior](https://www.postgresql.org)
    
# 3. Primeiros passos

### 1. Clonar os repositórios - Interface, Service User-NEW

```
git clone git@github.com:fga-eps-mds/2022-2-CAPJu-Interface.git && \
git clone git@github.com:fga-eps-mds/2022-2-CAPJu-Service.git && \
git clone git@github.com:fga-eps-mds/2022-2-CAPJu-User-NEW.git

```

### 2. Configurando .env

Configure o arquivo .env dos repositórios service e user-new igual abaixo:

```
POSTGRES_HOST=
POSTGRES_PORT=
POSTGRES_DATABASE=
POSTGRES_USER=
POSTGRES_PASSWORD=
JWT_SECRET=

```

Para o repositório interface configure o .env da seguinte forma:

```
JWT_SECRET=
API_SERVICE=
API_USER=
```

### 3. Instalado bibliotecas do node


Para instalar as bibliotecas de cada repositorio basta apenas dar o seguinte comando

```
yarn install
```

### 4. Executando o projeto

Para executar o projeto é recomendar executar os comandos na ordem de repositórios de back-end primeiro e front-end ao final. E cada um em um terminal diferente

```
yarn start
```


# Histórico de versões

| Data       | Versão | Descrição                                                                   | Autor                                        |
| ---------- | ------ | --------------------------------------------------------------------------- | -------------------------------------------- |
| 30/01/2023 | 1.0.0    | Adicionando roteiro execução do projeto                          | Antônio Aldísio                      |

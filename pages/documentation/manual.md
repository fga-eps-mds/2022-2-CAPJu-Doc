# Manual de instalação

# 1. Introdução

Essa sessão tem como objetivo orientar o passos a passos para rodar esse projeto em sua máquina local


# 2. Requisitos recomendados


## Hardware

- 6 GB de RAM
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

Crie um arquivo chamado .env no repositório raiz, em service e user-new, com o conteúdo igual ao demonstrado abaixo:

```
POSTGRES_HOST=
POSTGRES_PORT=
POSTGRES_DATABASE=
POSTGRES_USER=
POSTGRES_PASSWORD=
JWT_SECRET=

```

obs: as envs do POSTGRES são originadas de quando se monta o banco postgre.
obs²: a env JWT_SECRET deve ser igual em todos os repositórios.

Para o repositório interface configure o .env da seguinte forma:

```
JWT_SECRET=
API_SERVICE= <url do service>
```

### 3. Comandos para criar o banco e popular

É necessário estar no repositorio do service e executar o seguinte comando:

```
yarn migration &&  yarn seed
```
### 4. Instalado bibliotecas do node


Para instalar as bibliotecas de cada repositorio basta apenas executar o seguinte comando:

```
yarn install
```

### 5. Executando o projeto

Para executar o projeto é recomendado executar os comandos primeiramente nos repositórios de back-end e, em seguida no repositório de front-end. Tamém é recomendado que cada serviço utilize um terminal diferente. O comando utilizado para executar o projeto é o seguinte:

```
yarn start
```


# Histórico de versões

| Data       | Versão | Descrição                                      | Autor                                |
| ---------- | ------ | ---------------------------------------------- |------------------------------------- |
| 30/01/2023 | 1.0.0  | Adicionando roteiro execução do projeto        | Antônio Aldísio                      |
| 04/01/2023 | 1.0.1  | Revisão do documento                           | Fernando Miranda                     |
| 05/01/2023 | 1.0.2  | Revisão do documento²                          | Fernando Miranda                     |

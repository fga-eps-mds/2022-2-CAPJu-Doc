# CAPju 2022-2

# Treinamentos

- [Git](#Git)

## Contexto

Visando preparar a equipe de desenvolvimento para a execução do projeto, organizamos treinamentos sobre os principais conceitos a serem abordados no projeto para garantir o conhecimento da equipe sobre o mesmo.


## Git/GitHub

**Responsáveis**: [Fernado Miranda](https://github.com/ilus1)

**Data Realizada**: 10/11/2022

**Membros Participante na Vídeo Chamada**: Ana Luiza Rodrigues, Chaydson Ferreira, Lucas Lopes Frazão, Pedro Henrique Rodrigues de Carvalho e Samuel Gomes  

## Formato do Treinamento

Para melhor compreensão dos participantes do treinameto criamos um [repositório](https://github.com/ilus1/2022-2-CAPJu-Doc) para executar os comandos ao mesmo tempo que cada um era explicado. O treinamento foi realizado via Discord, onde cada integrante alterava parte do código de uma página e realizava o processo de commit para simular as atividades reais no dia a dia de desenvolvimento.

### Git

---

#### Iniciar um projeto

Para iniciar o git no seu projeto utilize o comando:

> git init

#### Obter um repositório

Para criar uma cópia de um trabalho em repositório remoto

> git clone usuário@servidor:/caminho/para/o/repositório

#### Adicionar arquivos alterados

> git add nome.ext

Para inserir mais de um arquivo no mesmo diretório

> git add diretório

#### Confirmar mudanças

> git commit -m "comentario"

##### Inserir Co-authored-by

> Co-authored-by: another-name <Coauther-name@example.com>"

#### Enviando alterações

> git push origin branch_name

#### Inserindo repositórorio remoto

> git remote add origin path

#### Ramificando

##### Para criar uma nova branch

> git checkout -b branch_name

##### Para alterar de branch

> git checkout branch_name

##### Para remover uma branch (LOCAL)

> git branch -d branch_name

#### Atualizar repositório local

> git pull

#### Visualizar commits

> git log

#### Fazer um backup das alterações que ainda não estão finalizadas

> git stash

---


**Histórico de Versão**

| Data       | Versão | Descrição                                        | Autor(es)       |
| ---------- | ------ | ------------------------------------------------ | --------------- |
| 10/11/2022 | 0.1.0    | Adicionando o treinamento de Git                 | Chaydson e Pedro|
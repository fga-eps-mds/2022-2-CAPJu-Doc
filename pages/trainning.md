# CAPju 2022-2

# Treinamentos

- [Git](#Git)

## Contexto

Visando preparar a equipe de desenvolvimento pra a execução do projeto, preparamos treinamentos sobre os principais conceitos a serem abordados no projeto para garantir o conhecimento da equipe sobre o mesmo.


## Git/GitHub

**Responsáveis**: [Fernado Miranda](https://github.com/ilus1)

**Data Realizada**: 10/11/2022

**Membros Participante na Vídeo Chamada**: Ana Luiza Rodrigues, Chaydson Ferreira, Lucas Lopes Frazão, Pedro Henrique Rodrigues de Carvalho e Samuel Gomes  

## Formato do Treinamento

Para melhor compreensão dos participantes do treinameto criamos um [repositório](https://github.com/FranciscoHeronildo/Treinamento-GIT-GITHUB) para executar os comandos ao mesmo tempo que cada um era explicado.

O Treinamento foi realizado via Microsoft Team e para os membros que não participaram foi disponibilizado a gravação da [chamava](https://drive.google.com/file/d/1c_pnLXBxgMqygQxqeAER0HN6f1jDSVk0/view?usp=sharing)
para que todos tenham acesso.

Além disso, foi proposto um desafio para fixaxão do conteúdo apresentado, desafio esse que encontra-se no repositório criado para o treinamento.


### Git

---

#### Iniciar um projeto

Para iniciar o git no seu projeto utilize o comando:

> git init

#### Obter um repositório

Para criar uma cópia de um trabalho em repositório remoto

> git clone usuário@servidor:/caminho/para/o/repositório

#### Adicionar arquivos alterados

> git add <arquivo>

Para inserir todos os arquivos modificados

> git add \*

#### Confirmar mudanças

> git commit -m "comentario"

> git commit -s

##### inserir Co-authored-by

> Co-authored-by: another-name <Coauther-name@example.com>"

#### Enviando alterações

> git push origin <branch>

#### Inserindo repositórorio remoto

> git remote add origin <path>

#### Ramificando

##### Para criar uma nova branch

> git checkout -b <branch_name>

##### Para alterar de branch

> git checkout <branch_name>

##### Para remover uma branch (LOCAL)

> git branch -d <branch_name>

#### Atualizar repositório local

> git pull

> git pull origin <branch_name>

#### Visualizar diferenças entre branch

> Git diff <branch1> <branch2>

#### Visualizar commits

> git log

#### Sobrescrever alterações locais

> git checkout -- <file>

#### Remover todas alterações locais

> git stash

---


**Histórico de Versão**

| Data       | Versão | Descrição                                        | Autor(es)       |
| ---------- | ------ | ------------------------------------------------ | --------------- |
| 10/11/2022 | 0.1.0    | Adicionando o treinamento de Git                 | Chaydson e Pedro|
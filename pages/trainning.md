# Treinamentos

- [Git](#gitgithub)
- [JavaScript](#javascript)
- [React](#react)

## Contexto

Visando preparar a equipe de desenvolvimento para a execução do projeto, organizamos treinamentos sobre os principais conceitos a serem abordados no projeto para garantir o conhecimento da equipe sobre o mesmo.

## Git/GitHub

**Responsáveis**: [Fernado Miranda](https://github.com/ilus1)

**Data Realizada**: 10/11/2022

**Membros Participante na Vídeo Chamada**: Ana Luiza Rodrigues, Chaydson Ferreira, Lucas Lopes Frazão, Pedro Henrique Rodrigues de Carvalho e Samuel Gomes

**Vídeo Chamada**: [[Parte 1](https://drive.google.com/file/d/14JDaRB8TPod8fIy9OHW0jV_BxwI4ACHT/view?usp=share_link)]

**Temas abordados**: Git clone, Git add, Git commit, Co-authored-by, Git push, Git remote, Git checkout -b, Git checkout, Git branch, Git branch -d,Git pull, Git log e Git stash.

## Formato do Treinamento

Para melhor compreensão dos participantes do treinameto criamos um [repositório](https://github.com/ilus1/2022-2-CAPJu-Doc) para executar os comandos ao mesmo tempo que cada um era explicado. O treinamento foi realizado via Discord, onde cada integrante alterava parte do código de uma página e realizava o processo de commit para simular as atividades reais no dia a dia de desenvolvimento.

---

### Tópicos Estudados

| Comando| Objetivo|
| --- | --- |
| git log                                   |  Visualizar commits                            |
| git pull                                  |  Atualizar repositório local                   |
| git stash                                 |  Arquivar alterações temporariamente           |
| git branch                                |  Vizualizar em qual branch se esta trabalhando |
| git clone **link**                        |  Criar uma cópia local do repositório remoto   |
| git add nome.ext                          |  Adicionar arquivos/diretorio                  |
| git commit -m "comentario"                |  Confirmar mudanças                            |
| git push origin branch_name               |  Enviar alterações                             |
| git remote add origin path                |  Inserir repositórorio remoto                  |
| git checkout -b branch_name               |  Criar uma nova branch e muda para ela         |
| git branch -d branch_name                 |  Remover uma branch local                      |
| git checkout branch_name                  |  Alterar de branch                             |
| Co-authored-by: name `<name@example.com>` |  Inserir Co-autor                              |

---

## JavaScript

**Responsáveis**: [Vitor Alves](https://github.com/vitorAlves7)

**Data Realizada**: 02/12/2022

**Members Participante na Vídeo Chamada**: Ana Luiza Rodrigues, Chaydson Ferreira, Lucas Lopes Frazão, Pedro Henrique, Samuel Gomes, Fernando Miranda e Davi Antônio

**Vídeo Chamada**: [[Parte 1](https://drive.google.com/file/d/1iKMJc3O8JG57jrkmkgCUrYf6dYB9Uheh/view?usp=sharing)] [[Parte 2](https://drive.google.com/file/d/1-ba1704PvQNB3dryGQTCs54rY-spp3Pz/view?usp=share_link)]

## Formato do Treinamento

O treinamento foi realizado via Discord, onde o responsável pela apresentação do conteúdo ([Vitor Alves](https://github.com/vitorAlves7)), demonstrava o funcionamento de cada tópico abordado, com o devído espaço para dúvidas dos participantes.

### Tópicos Estudados

| Comando| Objetivo|
| -- | --- |
| `var` |  Declaração de variáveis |
| `let` |  Declaração de variáveis |
| `const` |  Declaração de variáveis |
| `this` | Acesso a atributos dependendo do escopo tratado |
| `Arrow Functions` |  Passando funções como parametros para outras funções |
| `Destructuring` | Formas de acesso a atributos de objetos |
| `map` | Função que opera sobre todos os items de uma lista |
| `filter` |  Função que filtra uma lista dependendo da condição utilizada |
| `find` |  Retorna o primeiro item da lista que satisfaz a condição passada |
| `some` |  Retorna um boolean se algum item da lista satisfaz a condição passada |
| `sort` |  Ordena a lista dependendo da função utilizada |

---

## React

**Responsáveis**: [Fernando Miranda](https://github.com/ilus1)

**Data Realizada**: 15/12/2022

**Membros Participante na Vídeo Chamada**: Ana Luiza Rodrigues, Chaydson Ferreira, Lucas Lopes Frazão, Pedro Henrique e Samuel Gomes

**Vídeo Chamada**: [[Parte 1](https://drive.google.com/file/d/1XcH9vEZnTz5ybbnKZdVYkTQdslKv3Z3r/view?usp=share_link)]


## Formato do Treinamento

Durante o treinamento, o responsável pela apresentação do conteúdo ([Fernando Miranda]()) demonstra como se cria uma aplicação em react, e aborda todos os pontos citados abaixo.

### Tópicos Estudados

| Comando| Objetivo|
| -- | --- |
| `create-react-app` |  Criação de uma aplicação react |
| `npm install` |  Instala as dependências do projeto |
| `npm start` |  Inicia a aplicação react |
| `Single Page Application` |  Aplicação que não recarrega a página |
| `Debug via browser` |  Debugar a aplicação via browser |
| `Componentes` |  Componentes são blocos de construção de uma aplicação |
| `JSX` |  Linguagem de marcação que permite a criação de componentes |
| `Props` |  Propriedades de um componente |
| `Passagem de props` |  Passagem de props para um componente |
| `children` |  Acessando os filhos de um componente |
| `console.log` |  Imprimir no console do browser para debugar erros |
| `Interpolação` |  Inserção de lógica dentro da arvore html de um componente |
| `Template string` |  Inserção de variáveis em uma string |
| `useEffect` |  Executa uma função toda vez que o componente é renderizado |
| `useState` |  Cria um estado para o componente |
| `Códigos de status http` |  Códigos de status http |
| `short circuit` | Forma que o javascript trabalha com operadores && e || [Short circuit](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_AND) |



### Histórico de Versão

| Data       | Versão | Descrição                                        | Autor(es)       |
| ---------- | ------ | ------------------------------------------------ | --------------- |
| 10/11/2022 | 0.1.0  | Adicionando o treinamento de Git                 | Chaydson e Pedro|
| 08/12/2022 | 0.1.1  | Corrigir conceito do git checkout -b             | Davi            |
| 05/02/2023 | 1.0.0  | Atualização dos treinamentos oferecidos          | Fernando Miranda|

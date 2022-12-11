# Guia de Contribuição

Todo mundo é bem vindo para contribuir com o projeto CAPJu - Controle de Acompanhamento de Processos da Justiça. Mas é importante que as políticas de contribuição sejam seguidas antes de começar a contribuir.

## Quais são as políticas de contribuição do CAPJu?

* Leia o nosso [**Código de Conduta**](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/blob/main/.github/CODE_OF_CONDUCT.md)
* Crie sua [**Issue**](#crie-sua-issue)
* Siga a [**política de branches**](#política-de-branches)
* Siga a [**política de commits**](#política-de-commits)
* Crie um [**Pull Request**](#crie-um-pull-request)

---

## Crie seu Problema (_Issue_)

Para criar um novo problema (*issue*) é necessário seguir o [padrão](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/blob/main/.github/ISSUE_TEMPLATE/) criado para este projeto.

Antes de criar qualquer *issue*, verifique se já existe algo parecido na [lista de *issues*](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues).

Todos os problemas (*issues*) devem ser criados no [repositório de documentação](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc), mesmo que sejam referentes a histórias de usuário, tarefas, melhorias e correções de defeitos nos outros repositórios do projeto.

## Crie uma solicitação de *Pull/Merge* (*pull request*)

Para criar uma solicitação para que as modificações que realizou em sua ramificação sejam integradas ao código, é necessário seguir os passos abaixo: 

1. Primeiramente, é necessário que uma issue tenha sido criada na lista de [_Issues_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues).

2. Caso não exista, será preciso criar uma [_Nova Issue_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues/new/).

3. Todas as suas mudanças devem ser submetidas por meio de [_Pull Requests_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/pulls).

Recomenda-se adotar a [sintaxe para fechamento automático](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue) dos problemas (*issues*) assim que as modificações no código forem aceitas. Além disso, é recomendável que a mensagem da solicitação de mesclagem seja escrita já pensando que ela será incluída pelo GitHub no *merge commit*.

As políticas atuais exigem que no mínimo dois membros da equipe validem as modificações a serem aplicadas ao código. Apenas com a aprovação desse quórum que será possível aceitar as modificações e mesclá-las (*merge*) ao código na ramificação principal.

## Política de *Commits*

O sistema de controle de versões Git registra as modificações em objetos de *commit*, que guardam a diferença da versão anterior, metadados dos arquivos versionados que foram modificados, dados sobre o autor da modificação e uma texto detalhando a modificação, composta por título obrigatório e uma mensagem opcional.

### Mensagem do *Commit*

Para criar o *commit* é necessário seguir as seguintes regras:

* o título e a mensagem opcional dos *commits* devem estar em **português**
* o título do *commit* deve ser sucinto e objetivo, representando claramente o que está sendo alterado
* caso o *commit* seja composto por título e mensagem, deve haver o espaço de uma linha entre ambos

Além das regras acima, sugere-se também a aplicação das seguintes boas práticas na escrita do *commit*:

* limitar, se possível, o título em até cinquenta caracteres
* usar as descrições propostas pelos [*conventional commits*](https://www.conventionalcommits.org/en/v1.0.0/) para indicar o propósito do *commit*
* escrever o título de forma que fique claro o que acontecerá se o *commit* for aplicado
* escrever uma mensagem detalhando a modificação

## Rotulagem dos problemas (*Issues*)

Para mapear os conceitos de histórias de usuário, tarefas, defeitos e melhorias no sistema baseado em problemas (*issues*) do GitHub, adotou-se um sistema de rótulos ou etiquetas. Essas etiquetas devem ser usadas para categorizar todos os problemas (*issues*) que serão cadastrados no repositório.

### Rótulos disponíveis

Os seguintes rótulos foram cadastrados em todos os repositórios do projeto, já que são criados [automaticamente](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels) pelo GitHub:

- **`bug`**: indica um problema ou comportamento inesperados
- **`documentation`**: indica a necessidade de melhorias ou adições à documentação
- **`duplicate`**: indica problemas (*issues*), discussões ou solicitações de *pull/merge* semelhantes
- **`enhancement`**: indica pedidos para novas funcionalidades (*features*)
- **`good first issue`**: indica bons problemas (*issues*) para contribuidores iniciantes
- **`help wanted`**: indica que um mantenedor precisa de ajuda com um problema (*issue*) ou solicitação de *pull/merge*
- **`invalid`**: indica que um problema (*issue*), discussão, ou solicitação de *pull/merge* se tornou irrelevante
- **`question`**: indica que um problema (*issue*), solicitação de *pull/merge*, ou uma discussão precisam de mais informções
- **`wontfix`**: indica que o trabalho não continuará em um problema (*issue*), solicitação de *pull/merge* ou discussão

As etiquetas a seguir também são cadastradas em todos os repositórios, mas são customizadas e possuem cores determinadas na notação HTML (valores hexadecimais dos canais vermelho, verde e azul com resolução de 8 bits):

- **`HOTFIX`** (cor `#d73a4a`): indica uma correção de defeitos críticos
- **`DOCS`** (cor `#0075ca`): indica a aplicação de melhorias ou adições à documentação do projeto
- **`FEATURE`** (cor `#094EF2`): indica a introdução de uma funcionalidade nova
- **`US`** (cor `#BE71F6`): indica que o problema (*issue*) é uma história de usuário (*user story*)
- **`ARQ`** (cor `#0D5571`): indica mudanças na arquitetura da aplicação ou de um de seus módulos ou serviços
- **`DEVOPS`** (cor `#9014A0`): indica mudanças na esteira de integração e disponibilização contínua
- **`ANALYTICS`** (cor `#12477F`): indica mudanças nos analisadores estáticos
- **`EASY`** (cor `#C5DEF5`): indica que o problema tem uma dificuldade baixa
- **`MEDIUM`** (cor `#BFD4F2`): indica que o problema possui um grau médio de dificuldade
- **`HARD`** (cor `#D4C5F9`): indica que o problema possui um alto grau de dificuldade
- **`EPS`** `#006633`: indica que o problema será trabalhado por alunos da disciplina de Engenharia de Produto de Software (EPS)
- **`MDS`** (cor `#0068b4`): indica que o problema será trabalhado por alunos da disciplina de Métodos de Desenvolvimento de Software (MDS)

## Política de Ramificações (*branches*)

Objetivando facilitar a execução da disciplina de Gerência de Configuração de Software, optou-se pelo estabelecimento de uma Política para regulamentar o uso do recurso de ramificações (*branches*) do sistema de controle de versões Git. A Política escolhida é baseada na [Gitlab FLow](https://docs.gitlab.com/ee/topics/gitlab_flow.html), que conta com ramificações para implementação de novas funcionalidades [(*feature branches*)](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow), uma *branch* para estabilização do código e integração das funcionalidades, e outra para versionar código de produção, que passou por testes e validação do cliente. Como haverá somente uma versão estável em uso pelo cliente, optou-se por não usar múltiplas *branches* de produção.

### A ramificação principal (`main`)

A *branch* principal, `main`, hospeda o código estável do projeto em todos os repositórios. Todos os *commits* na `main` implementam as funcionalidades de maneira que já possam ser executadas em ambiente de produção. Além disso, eles são todos oriundos da *branch* de homologação e integração de funcionalidades, a `devel`.

As novas versões (*releases*) são lançadas através da marcação com rótulos anotados [(*annotaded tags*)](https://git-scm.com/book/en/v2/Git-Basics-Tagging) do Git. Prefere-se o uso dos rótulos anotados, gerados pelo comando `git tag -a nome-tag`, aos rótulos comuns (*lightweight tags*), gerados pelo `git tag nome-tag`, pois são objetos separados no sistema de versão, e guardam dados de quem os gerou.

### Ramificação para página Web

A *branch* `gh-pages` é usada para disponibilizar a documentação do projeto em formato de página Web. Essa documentação é hospedada em um repositório específico, sendo disponibilizada pelo serviço [Github Pages](https://fga-eps-mds.github.io/2022-2-CAPJu-Doc/#/).

### Ramificação para integração e homologação (`devel`)

A *branch* `devel` será usada para integração de novas funcionalidades e homologação. Ela é inicializada a partir da `main`, e continua paralela a essa integrando as novas funcionalidades. Quando o código é homologado, ocorre uma operação de mesclagem (*merge*) da `devel` na `main`.

### Ramificações para novas funcionalidades (*feature branches*) de documentação

No repositório de documentação, as funcionalidades, modificações ou adições aos documentos do projeto, são iniciadas nas ramificações que possuem o nome que segue o padrão: `docs/<issue-id>-<desrição>`. Assim como nos outros repositórios, tais modificações são integradas na *branch* `devel` antes de serem disponibilizadas na `main` e, no caso específico da documentação, como página web na ramificação `gh-pages`.

**Exemplo**: `docs/1-inicializa-repositorio`

### Ramificações para novas funcionalidades (*feature branches*) gerais

Há outras situações previstas para o uso das ramificações de novas funcionalidades: aplicar correções urgentes, melhorias, refatorações ou implementar funcionalidades novas. É importante nomear as *branches* conforme o padrão indicado na política, pois após serem integradas na `devel`, estas serão apagadas, e serão documentadas somente com seus nomes nos *merge commits*.

Abaixo segue a lista dos padrões de nomenclatura e os respectivos tipos de funcionalidade:

* **`hotfix/<issue-id>-<nome_bug>`**: usado para funcionalidades de correção de defeitos. É preciso especificar o número da *issue* cadastrada no repositório de documentação.
**Exemplo**: `hotfix/1-tela-inexistente`

* **`enhacement/<issue-id>-<nome_bug>`**: usado para melhoria de funcionalidades já presentes na aplicação. É preciso especificar o número da *issue* cadastrada no repositório.
**Exemplo**: `enhacement/1-adiciona-icones`

* **`feature/<issue-id>-<feature-name>`**: usado para funcionalidades novas. O nome deve conter o número da *issue* registrada, no formato.
**Exemplo**: `feature/1-estrutura-generica-de-listas-ligadas`

* **`refactor/<nome_refatoracao>`**: usado para ajustes no código que não corrigem defeitos e nem adicionam novas funcionalidades.
**Exemplo**: `refactor/daos`


## Referência

> Guia de Contribuição [Capju 2022-1](https://github.com/fga-eps-mds/2022-1-CAPJu-Doc/blob/main/.github/CONTRIBUTING.md)

## Histórico de Versão

| Data       | Versão   | Descrição                                               | Autor(es)       |
| ---------- | ------   | ------------------------------------------------------- | --------------- |
| 10/11/2022 | 0.1.0    | Criação do documento                                    | Paulo Batista   |
| 15/11/2022 | 0.1.1    | Ajustar documento                                       | Paulo Batista   |
| 23/11/2022 | 0.2.0    | Nova política de padrão para melhorias                  | Lude Ribeiro    |
| 08/12/2022 | 0.2.1    | Corrigir item de lista formatado como parágrafo         | Davi Antônio    |
| 09/12/2022 | 0.2.2    | Explicar rótulos, inclusão de *issues* e escrita de PRs | Davi Antônio    |

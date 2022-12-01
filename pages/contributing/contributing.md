
# Guia de Contribuição

Todo mundo é bem vindo para contribuir com o projeto CAPJu - Controle de Acompanhamento de Processos da Justiça. Mas é importante que as políticas de contribuição sejam seguidas antes de começar a contribuir.

## Quais são as políticas de contribuição do CAPJu?

<!-- * Leia o nosso [**Código de Conduta**](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/blob/main/.github/CODE_OF_CONDUCT.md) -->
* [**Issue**](#crie-sua-issue)
* [**Política de branches**](#política-de-branches)
* [**Política de commits**](#política-de-commits)
* [**Pull Request**](#crie-um-pull-request)

## Crie sua _Issue_

* Para criar um nova issue é necessário seguir o template da [_issue_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/blob/main/.github/ISSUE_TEMPLATE/) que foi criado para este projeto. Antes de criar qualquer issue, verifique se já existe alguma parecida que já foi criada na [_lista de issues_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues).

## Crie um Pull Request

1. Primeiramente, é necessário que uma issue tenha sido criada na lista de [_Issues_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues).

2. Caso não exista, será preciso criar uma [_Nova Issue_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues/new/).

3. Todas as suas mudanças devem ser submetidas por meio de [_Pull Requests_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/pulls).

## Política de _Commits_

### Mensagem do _Commit_

Para criar o commit é necessário seguir as seguintes regras:

* A descrição dos _commits_ devem está em **português**
* A descrição do commit deve ser sucinta e objetiva, representando claramente o que está sendo alterado naquele _commit_.

> `git commit -m 'Mensagem'`

* No caso de uma correção de bugs, a mensagem deve começar com hotfix.

> `git commit -m 'hotfix-Mensagem'`

## Política de _Branches_

Com o intuito de possuir uma melhor dinâmica de mudanças de código, é importante que tenhamos uma boa política de branches. Este documento servirá de base para criação de branches e como serão organizadas, estas baseadas no git flow que é um modelo de organização de branches.

* **Branch main**: Esta será a branch que contém o código em nível de produção, será o código mais consolidado existente na aplicação. Todo o código novo produzido eventualmente é juntado com a branch master, em algum momento do desenvolvimento;

* **Branch develop**: Develop é a branch que logo após releases deverá ser identica à master, porém, quando as features são terminadas, elas são juntadas nesta branch, testadas e somente depois as atualizações da develop passam pelo processo de juntar as novas atualizações com a branch master;

* **Branches feature** - Essas são as branches na qual são desenvolvidos novos recursos ao projeto, elas serão criadas com o nome começando **feature/** (exemplo: feature/new-layout) e a partir da branch develop, e, ao final, são juntadas com a branch develop;

* **Branches hotfix** - São branches no qual são realizadas correções de bugs críticos encontrados em ambiente de produção, e que por isso são criadas a partir da branch master, e são juntadas diretamente com a branch master e com a branch develop. Por convenção, essas branches tem o nome começando com **hotfix/** e terminando com o próximo sub-número de versão (exemplo: hotfix/2.31.1);

* **Branches release** - São branches com um nível de confiança maior do que a branch develop, e que se encontram em nível de preparação para ser juntada com a branch master e com a branch develop, nessas branches, bugs encontrados durante os testes das features que vão para produção podem ser corrigidos mais tranquilamente, antes de irem efetivamente para produção. Por convenção, essas branches tem o nome começando com **release/** e terminando com o número da próxima versão do software, exemplo (release/2.32.0)

* **Branches docs** - Essas são as branches na qual são desenvolvidos os documentos do projeto, elas serão criadas com o nome começando **docs/** (exemplo: documentation/documento-visao), elas são criadas a partir da branch develop e, ao final, é feito um pull-request para a branch develop.

* **Branch gh-pages**: Designada para conter todos os documentos do projeto, disponíveis no [Github Pages](https://fga-eps-mds.github.io/2022-2-CAPJu-Doc/#/)


## Referência

> [Gitflow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

> [Guia de Contribuição Capju 2022-1](https://github.com/fga-eps-mds/2022-1-CAPJu-Doc/blob/main/.github/CONTRIBUTING.md)

**Histórico de Versão**

| Data       | Versão | Descrição                                        | Autor(es)       |
| ---------- | ------ | ------------------------------------------------ | --------------- |
| 10/11/2022 | 0.1.0    | Criação do documento              | Paulo Batista |
| 15/11/2022 | 0.1.1    | Ajustar documento              | Paulo Batista |
| 01/12/2022 | 0.1.2    | Ajustar documento              | Antonio Aldisio |

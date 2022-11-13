
# Guia de Contribuição

Todo mundo é bem vindo para contribuir com o projeto CAPJu - Controle de Acompanhamento de Processos da Justiça. Mas é importante que as políticas de contribuição sejam seguidas antes de começar a contribuir.

## Quais são as políticas de contribuição do CAPJu?

* Leia o nosso [**Código de Conduta**](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/blob/main/.github/CODE_OF_CONDUCT.md)
* Crie sua [**Issue**](#crie-sua-issue)
* Siga a [**política de branches**](#política-de-branches)
* Siga a [**política de commits**](#política-de-commits)
* Crie um [**Pull Request**](#crie-um-pull-request)

---

## Crie sua _Issue_

* Para criar um nova issue é necessário seguir o template da [_issue_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/blob/main/.github/ISSUE_TEMPLATE/) que foi criado para este projeto. Antes de criar qualquer issue, verifique se já existe alguma parecida que já foi criada na [_lista de issues_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues). 

## Crie um Pull Request

1. Primeiramente, é necessário que uma issue tenha sido criada na lista de [_Issues_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues).

2. Caso não exista, será preciso criar uma [_Nova Issue_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/issues/new/).

3. Todas as suas mudanças devem ser submetidas por meio de [_Pull Requests_](https://github.com/fga-eps-mds/2022-2-CAPJu-Doc/pulls).

## Política de _Commits_

### Mensagem do _Commit_

Para criar o commit é necessário seguir as seguintes regras:
- A descrição dos _commits_ devem está em **português** 
- A descrição do commit deve ser sucinta e objetiva, representando claramente o que está sendo alterado naquele _commit_.
- Caso não seja apenas um correção de bugs, a mensagem deve apresentar o número da issue como no exemplo abaixo:
> `git commit -m 'issueId-Mensagem'`

- No caso de uma correção de bugs, a mensagem deve começar com hotfix.
> `git commit -m 'hotfix-Mensagem'`

## Política de _Branches_

Objetivando manter a confiabilidade do código fonte do nosso produto, propõe-se o uso de uma política de branches para orientar os desenvolvedores no modo de organização das suas contribuições neste repositório. Assim, estabelecemos:


branch padrão **main**, para hospedar o código estável do projeto (que estará em ambiente de homologação);


__gh-pages__: Designada para conter todos os documentos do projeto, disponíveis no [Github Pages](https://fga-eps-mds.github.io/2022-2-CAPJu-Doc/#/)

* __`docs/nome_documento`__ - Branch onde será consolidada a documentação do projeto, sendo usada exclusivamente para isso.

* __`devel`__ - Branch destinada à integração das novas funcionalidades desenvolvidas, onde estarão as features em estágio avançado e/ou completas. Esta será a branch base para o desenvolvimento inicial de features e de correção de bugs. 

* __`hotfix/<nome_bug>`__ - Branch dedicada para correção de bugs presentes na aplicação. É preciso especificar o número da _issue_ cadastrada no repositório.
Exemplo: `hotfix/1-<nome_bug>` (_issue_ #1)

* __`feature/<feature-name>`__ - Branch usada para desenvolvimento de uma nova feature no projeto. O nome deve conter o número da issue registrada, no formato. 
Exemplo: `feature/1-<feature-name>` (_issue_ #1)

* __`release/<release-version>`__ - Branch destinada à ajustes finais/build que serão feitas para entrega de uma realize do software. O nome deve ser a própria versão da release. 

## Referência:

> Guia de Contribuição [Over26](https://github.com/fga-eps-mds/2022-1-CAPJu-Doc/blob/main/.github/CONTRIBUTING.md)
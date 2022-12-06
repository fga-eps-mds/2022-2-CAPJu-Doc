# Planejamento de Qualidade

## Introdução

Segundo a ISO/IEC 25010 a "Qualidade de um sistema é o grau em que o sistema satisfaz as necessidades declaradas e implícitas de suas várias partes interessadas e, portanto, fornece valor. Essas necessidades dos stakeholders (funcionalidade, desempenho, segurança, manutenibilidade etc.) são justamente o que está representado no modelo de qualidade, que categoriza a qualidade do produto em características e subcaracterísticas". Dessa forma, com o objetivo de detectar as não conformidades dentro do projeto e estabelecer ações corretivas e preventivas para entregar um produto que possua um grau elevado de satisfação para o usuário final, serão abordados neste Planejamento de Qualidade, práticas, modelos e parâmetros que permitam ao time atingir esse objetivo.

Este documento usa como apoio o modelo de qualidade Q-Rapids que busca a integração de fontes de dados heterogêneas, a agregação e interpretação de dados brutos e a seleção de métricas relevantes e orientadas para o negócio, usamos também o [notebook](https://github.com/fga-eps-mds/2022-1-CAPJu-Doc/blob/main/analytics.ipynb) da disciplina para apoiar as análises de dados da qualidade. Além disso, em paralelo utilizamos também a abordagem **GQM** (Goal Question Metrics) que é uma abordagem de cima para baixo (top-down) que estabelece um sistema de medição direcionado a metas para desenvolvimento de software em que a equipe inicia com metas organizacionais, define a medição das metas, levanta questões a abordar os objetivos e identifica as métricas que proporcionem as respostas. O modelo GQM está dividido em três níveis: Nível Conceitual, nível Operacional e nível Quantitativo.

Essa abordagem possui 3 níveis hierárquicos, são eles:

**Conceitual (Objetivos):** Uma meta é definida para algum objeto de medição, esse objeto pode ser produtos, processos ou recursos.<br>
**Operacional (Questões):** Elaborar perguntas que nos ajudam a caracterizar o objeto de medição e nos ajuda a escolher o ponto de vista da análise de qualidade que será feita.<br>
**Quantitativo (Métricas):** Conjunto de dados que está associado às perguntas a fim de respondê-las.

## Objetivos

Para definição dos nossos objetivos de qualidade separamos a qualidade em duas categorias, sendo elas: Qualidade de Projeto e Qualidade de Produto.

## Qualidade do Projeto

### Objetivo 1 - Medir a Qualidade Organizacional do time

Para que seja possível medir a qualidade interna organizacional é necessário primeiramente definir os aspectos que serão avaliados dentro desse contexto. Avaliaremos dentro do Objetivo 1, por exemplo, a participação do time nas cerimônias do Scrum e capacidade de entrega do time. A medição da qualidade a nível organizacional permite ao próprio time uma autonomia para tomar decisões e gerar uma melhoria contínua nas entregas de releases.

Conforme propõe a ISO/IEC 14598-1 que está direcionada ao ponto de vista de desenvolvedores que pretendem desenvolver um novo produto ou melhorar um produto existente e pretendam executar avaliação de produto utilizando pessoas de seu próprio corpo técnico pode-se fazer o uso de indicadores que ajudam a prever a qualidade do produto final através da medição de produtos intermediários desenvolvidos durante o ciclo de vida.

Para medirmos a participação do time nas cerimonias do Scrum, inicialmente coletamos a cada reunião de _Retrospective_ e _Planning_ o relatório de presença gerado pela plataforma _Microsoft Teams_. Após esse passo, o time de EPS definiu uma escala própria para obter os resultados da participação do time nas reuniões de acordo com a tabela abaixo:

| Escala de Participação | Significado |
| ---------------------- | ----------- |
| De 0% a 70%            | Ruim        |
| De 70% a 90%           | Boa         |
| De 90% a 100%          | Ótima       |

Para obtermos métricas de qualidade a nível organizacional, foram escolhidos os seguintes aspectos para serem avaliados:

| Goal | Questions | Metrics |
| ---- | --------- | ------- |
| 1    | Qual é a frequência de participação dos membros nas cerimonias do Scrum? Com que velocidade o time realiza entregas? | Velocity, Escala de participação nas cerimonias do Scrum |

### Resultados da métrica de participação

| Data da reunião | Porcentagem de participação |
| --------------- | --------------------------- |
| 12/07           | 100%                        |

### Resultados da métrica de capacidade de entrega do time

#### Velocity

O Velocity é utilizado para medir a quantidade média de trabalho que uma equipe pode completar em um “ciclo de entrega” – normalmente um sprint.

## Qualidade do Produto

### Objetivo 2 - Medir a Qualidade externa do Software

Para avaliar a qualidade externa do software, que ocorre quando o software sendo testado em um ambiente simulado, serão coletadas métricas por meio do SonarCloud após cada _Pull Request_ submetido e cujo _merge_ tenha sido realizado. Após coletadas, essas métricas são combinadas para calcular cada um dos aspectos de qualidade que interessa a este Projeto, estando esses divididos em:

- Manutenibilidade do código
- Confiabilidade

| Goal | Questions | Metrics |
| ---- | --------- | ------- |
| 2    | O código é reaproveitado? O código é legível? Após inserir novas funcionalidades é fácil identificar bugs? | files,functions, complexity, comment_lines_density, duplicated_lines_density, coverage, ncloc, tests, test_errors, test_failures, test_execution_time, security_rating |

### Aspecto Manutenibilidade

#### Fator _Code Quality_

O conjunto de métricas abaixo, referentes ao fator de qualidade _Code Quality_ que compõe o aspecto de qualidade Manutenibilidade, será coletado para avaliar a manutenibilidade do código do projeto. Tal aspecto é importante por nos permitir avaliar o quão fácil será realizar a manutenção no código do projeto.

1. **Complexidade**

Essa métrica tem por objetivo identificar a densidade de arquivos não complexos, sendo estes definidos como os arquivos que estão fora do limite de complexidade ciclomática definido (por padrão 10).

<!-- <p align="center">
<strong>Densidade de arquivos não complexos</strong>
<br>

<img src="https://i.imgur.com/FWmlxJG.png">

<br>
Fonte: Próprio autor
</p>

Obs.: onde um arquivo complexo é definido como aquele cuja complexidade ciclomática por função é maior que 10 (valor padrão). A Complexidade Ciclomática contabiliza quantos caminhos possíveis um fluxo inicial de código pode assumir. -->

2. **Comentários**

Essa métrica tem como objetivo identificar a densidade de arquivos comentados. Um arquivo é tido como comentado se a sua densidade de linhas comentadas estiver dentro do limite definido (entre 10% e 30% por padrão).

<p align="center">
<strong>Densidade de arquivos comentados</strong>
<br>

<img src="https://i.imgur.com/HcSasIK.png">

<br>
Fonte: Próprio autor
</p>

<p align="center">
<strong>Densidade de linhas comentadas</strong>
<br>

<img src="https://i.imgur.com/XAxupgE.png">

<br>
Fonte: Próprio autor
</p>

3. **Duplicidade**

Essa métrica avalia a quantidade de arquivos abaixo do limite definido para a porcentagem de linhas duplicadas. Onde, um arquivo é definido como não havendo duplicações se a sua densidade de duplicação é menor que 5% (valor padrão estabelecido).

<p align="center">
<strong>Ausência de duplicações</strong>
<br>

<img src="https://i.imgur.com/7wlLy4D.png">

<br>
Fonte: Próprio autor
</p>

<p align="center">
<strong>Densidade de duplicação</strong>
<br>

<img src="https://i.imgur.com/em1EJmF.png">

<br>
Fonte: Próprio autor
</p>

### Cálculo Manutenibilidade e Interpretação

Tendo cada uma das 3 métricas acima calculadas partimos para o cálculo do fator de qualidade _Code Quality_, sendo o único fator de qualidade que compõe o aspecto de qualidade Manutenibilidade e, portanto, seu resultado definirá tal aspecto. O cálculo é definido como:

<p align="center">
<strong>Manutenibilidade (Qualidade de Código)</strong>
<br>

<img src="https://i.imgur.com/rhLy38Y.png">

<br>
Fonte: Próprio autor
</p>

<p align="center">
<strong>Constantes na Equação Qualidade de Código</strong>
<br>

<img src="https://i.imgur.com/K7ifyHE.png">

<br>
Fonte: Próprio autor
</p>

Onde, m1, m2 e m3 remetem a Complexidade, Comentários e Duplicidade, respectivamente. O resultado final é um valor entre 0 e 1 (0: péssimo, 1: excelente)

#### Aspecto Confiabilidade

Para mensurar esse aspecto é necessário antes o cálculo do fator de qualidade _Testing Status_. Esse aspecto é importante para avaliar o quão confiável o código é em realizar aquilo que propõe.

#### Fator _Testing Status_

A fim de mensurá-lo, são necessárias 3 métricas: _Passed Tests_, _Fast Test Builds_ e _Test Coverage_.

1. **_Passed tests_**

Calcula a densidade de testes unitários com sucesso. É definida como:

<p align="center">
<strong>Quantidade de testes com sucesso</strong>
<br>

<img src="https://i.imgur.com/s444taf.png">

<br>
Fonte: Próprio autor

</p>

2. **_Fast Test Builds_**

Tem como objetivo o cálculo das _builds_ de teste cuja duração esteja abaixo do limite definido (300 segundos).

<p align="center">
<strong>Construções de teste rápidas</strong>
<br>

<img src="https://i.imgur.com/nSRTZ2y.png">

<br>
Fonte: Próprio autor
</p>

Obs.: _fast unit test_ são os testes cuja duração de execução está abaixo de 300 segundos.

3. **_Test Coverage_**

Avalia a cobertura de código do Projeto considerando os arquivos de teste unitários que estejam acima do limite definido (60% por padrão).

<p align="center">
<strong>Cobertura de código</strong>
<br>

<img src="https://i.imgur.com/pi1v4yS.png">

<br>
Fonte: Próprio autor
</p>

Obs.: Onde _AcceptedUnitTestFiles_ são aqueles arquivos de teste unitário que testam ao menos 60% do código de seu componente alvo para o qual foi implementado.

### Cálculo Confiabilidade e Interpretação

Finalmente partimos para o cálculo do fator de qualidade _Testing Status_ que, por ser o único fator de qualidade que compõe o aspecto Confiabilidade, definirá o seu valor final.

<p align="center">
<strong>Cálculo fator Testing Status</strong>
<br>

<img src="https://i.imgur.com/jLAYQMS.png">

<br>
Fonte: Próprio autor
</p>

<p align="center">
<strong>Constantes na equação Testing Status</strong>
<br>

<img src="https://i.imgur.com/maI6Byh.png">

<br>
Fonte: Próprio autor
</p>

Onde, m4, m5 e m6 remetem a _Passed Tests_, _Fast Test Builds_ e _Coverage_, respectivamente. O resultado final é um valor entre 0 e 1 (0: péssimo, 1: excelente)

### Objetivo 3 - Medir a Qualidade do Software em Uso

É importante considerar que o cliente é quem está à frente. Ele tem o direito de participar e opinar durante o processo de construção do software. Neste contexto, a experiência do usuário, além das qualidades técnicas do software, é um fator determinante para a construção de sistemas de maior qualidade. Sua participação pode facilitar a compreensão dos seus desejos quanto ao software que está sendo desenvolvido. Esse aspecto da qualidade do software é chamado usabilidade.

Dessa forma, para medirmos a qualidade do nosso software em uso seria necessário termos finalizado o desenvolvimento do software e disponibilizado para os usuários finais, no entanto, no momento isso não ase aplica, visto que ainda estamos em fase de desenvolvimento e sem acesso aos usuários finais. Mas futuramente pretendemos realizar testes de usabilidade com os usuários finais.

| Goal | Questions | Metrics |
| ---- | --------- | ------- |
| 3    | Qual o nível de satisfação do cliente ao navegar por cada funcionalidade? | Respostas dos testes de usabilidade via formulário |

## Histórico de Versão

| Data | Versão | Descrição | Autor(es) |
| ---- | ------ | --------- | --------- |
| 05/12/2022 | 0.1 | Criação do plano de qualidade | Lude Ribeiro |

## Referências

> RODRIGUES, Claudia. A importância de um plano de qualidade de software e a estratégia de testes. Linkedin, 2017. Disponível em: <https://www.linkedin.com/pulse/import%C3%A2ncia-de-um-plano-qualidade-software-e-testes-farias-ctfl/?originalSubdomain=pt>. Acesso em: 30 de jul. de 2022.
> ARIAS, Raphael. Como criar um plano de gerenciamento da qualidade. Excellence Blog, 2020. Disponível em: <https://blog.softexpert.com/plano-gerenciamento-qualidade/>. Acesso em: 30 de jul. de 2022.
> SILVA, C. V. P. GQM - Goal Question Metric. Ago 2009. Disponível em: <https://www.cin.ufpe.br/~scbs/metricas/seminarios/GQM_texto.pdf> Acesso em: 30 jul. 2022.
> CAMPOS, Fábio. Qualidade, Qualidade de Software e Garantia da Qualidade de Software são as mesmas coisas?. Linha de Código, 2022. Disponível em: <http://www.linhadecodigo.com.br/artigo/1712/qualidade-qualidade-de-software-e-garantia-da-qualidade-de-software-sao-as-mesmas-coisas.aspx>. Acesso em: 30 jul. 2022.
> LENILDO. Qualidade de Software - Engenharia de Software 29. DEVMEDIA, 2010. Disponível em: <https://www.devmedia.com.br/qualidade-de-software-engenharia-de-software-29/18209>. Acesso em: 30 jul. 2022.
> ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. NBR ISO/IEC 25010: Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — System and software quality models, 2011.
> QuestionPro. Question Pro, 2022. Blog de pesquisa online e inteligẽncia de mercado. Disponível em: <https://www.questionpro.com/blog/pt-br/exemplos-de-escalas-likert/>. Acesso em: 10 set. 2022.
> Fernandez, S. M. Jedlitschka, A. Guzman, L. Vollmer, A. M. A Quality Model for Actionable Analytics in Rapid
> Software Development. 2018 44th Euromicro Conference on Software Engineering and Advanced Applications. Kaiserslautern, Germany, 2018. Disponível em: <https://ieeexplore.ieee.org/abstract/document/8498234?casa_token=8aE9OufxCwwAAAAA:0LeENRkDbLsapTL2LvdAXVk1pv2PMfMoAa1auLEu1OOqsAD0guuZnLG3V36Bf0JgGgkXnb7YqHE>

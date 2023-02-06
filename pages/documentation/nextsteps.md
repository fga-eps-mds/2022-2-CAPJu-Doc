# Próximos passos

## 1. Introdução

Essa documento tem como objetivo dar um guia dos próximos passos que pode e/ou devem ser executados no projeto que não puderam ser executados no semestre de 2022-2.

## 2. Front-End

No repositório da [interface](https://github.com/fga-eps-mds/2022-2-CAPJu-Interface) recomendamos:

- Refatorção de todo os arquivos usando as boas práticas do [REACT](https://reactjs.org/);
- Aumento de cobertura de teste;
- Realizar teste de cobertura de borda;
- Ajustar tempo do token;
- Modularizar o código;
- Utilizar componentização:
    - Principalmente nas modais do sistema;
- Padronizar coluna de ações em todas as tabelas;
- Adicionar opção de deletar unidade(Conferir com o cliente);
- Corrigir endpoint de recuperação de fluxos(retornar lista de usuários cadastrados);
- Melhorar visual das dropdowns do sistema(gerar protótipo e apresentar pro cliente);

## 3. Back-End

No repositório do [user-new](https://github.com/fga-eps-mds/2022-2-CAPJu-user-new) recomendamos:

- Adequação do escopo desse microserviço (Rotas se encontra dentro do Service);
- Criação de testes;
- Melhora o swagger;

No repositório do [service](https://github.com/fga-eps-mds/2022-2-CAPJu-service) recomendamos:

- Criação de Swagger;
- Melhoria de mock do banco de dados;
- Aumento da cobertura de testes;
- Retira vestígio do mongoDB;
- Desenvolver rotas mais genérica e utilizar filtro para fazer as pesquisas;
- Usar uma criptrografia melhor para a senha;
- Ajustar tempo do token;

## Histórico de versão

| Data | Versão | Descrição | Autor(es) |
| ---- | ------ | --------- | --------- |
| 03/02/2023 | 0.1.0 | Criação do documento | Antônio Aldísio |
| 06/02/2023 | 1.0.0 | Revisão do documento | Fernando M.     |

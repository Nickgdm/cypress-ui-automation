<pre>
╔═════════════════════════════════════════════════════════════════════════════════════════════════════════╗
║                                 AUTOMAÇÃO DE TESTES DE UI — HUB DE LEITURA                              ║
╚═════════════════════════════════════════════════════════════════════════════════════════════════════════╝
</pre>

Projeto de estudo voltado à automação de testes end-to-end da interface web da aplicação Hub de Leitura, utilizando Cypress.

## SOBRE O PROJETO

O repositório reúne testes automatizados de interface para praticar a validação de fluxos de usuário e o comportamento da aplicação em cenários reproduzíveis.

##OBJETIVOS

- Automatizar fluxos da interface web.
- Validar comportamentos da aplicação por meio de cenários reproduzíveis.
- Praticar a organização, a configuração e a execução de testes de UI.
- Explorar a possibilidade de integrar a execução dos testes a um pipeline de integração contínua.

## TECNOLOGIAS E FERRAMENTAS

- JavaScript
- Node.js e npm
- Cypress
- Jenkinsfile, presente no repositório, como ponto de partida para integração contínua

## PRÉ-REQUISITOS

- Node.js e npm instalados.
- Aplicação Hub de Leitura em execução e acessível pela URL configurada nos testes.
- Dependências do projeto instaladas.

## INSTALAÇÃO E EXECUÇÃO

Instale as dependências:

```bash
npm install
```

Abra a interface do Cypress:

```bash
npx cypress open
```

Execute os testes em modo headless:

```bash
npx cypress run
```

Consulte o arquivo `package.json` para confirmar os scripts disponíveis e verifique `cypress.config.js` e os arquivos de teste em `cypress/` para conhecer a configuração e os cenários implementados.

Se utilizar o Cypress Cloud para registrar execuções, configure a variável de ambiente `CYPRESS_RECORD_KEY` localmente antes de executar o script de relatório correspondente. Não inclua chaves ou credenciais no código nem no repositório.

## ESTRUTURA DO PROJETO

```text
hub-de-leitura-teste-ui/
├── .github/
├── cypress/
├── cypress.config.js
├── jenkinsfile
├── package.json
├── package-lock.json
└── README.md
```

A estrutura acima representa os principais diretórios e arquivos documentados neste projeto.

## DESAFIOS PRÁTICOS

- Preparar a aplicação utilizada como alvo dos testes.
- Selecionar elementos da interface de forma adequada.
- Simular ações realizadas por usuários.
- Validar estados e comportamentos da interface sem depender de esperas arbitrárias.
- Considerar como os testes podem ser executados em um fluxo de integração contínua.

## BOAS PRÁTICAS

- Manter os testes organizados em diretório próprio.
- Separar a configuração do Cypress dos cenários de teste.
- Consultar a configuração do ambiente antes de executar a suíte.
- Não armazenar chaves, senhas ou outros segredos no repositório.
- Confirmar os resultados por meio da execução real dos testes, sem presumir que todos passam.

## APRENDIZADOS

A atividade permite praticar automação end-to-end com Cypress, desde a preparação do ambiente e a seleção de elementos até a validação dos comportamentos da interface. A presença de um Jenkinsfile também oferece uma oportunidade de estudo sobre a integração de testes a um fluxo de CI.

## CONSIDERAÇÕES FINAIS

A execução depende da disponibilidade da aplicação Hub de Leitura e da correspondência entre a URL configurada e o ambiente utilizado. Consulte os arquivos de teste para identificar os cenários implementados e eventuais configurações adicionais necessárias.
<pre>
╔═════════════════════════════════════════════════════════════════════════════════════════════════════════╗
║       Atividade desenvolvida durante a formação profissionalizante em Quality Assurance (QA) pela       ║
║                     EBAC — Escola Britânica de Artes Criativas e Tecnologia                             ║
╚═════════════════════════════════════════════════════════════════════════════════════════════════════════╝
</pre>

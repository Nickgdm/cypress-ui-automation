# Automação de Testes de UI — Hub de Leitura

Projeto de automação de interface para a aplicação Hub de Leitura, utilizando Cypress para executar cenários end-to-end.

## Objetivos
- Automatizar fluxos da interface web.
- Validar o comportamento da aplicação por meio de cenários reproduzíveis.
- Praticar organização, configuração e execução de testes de UI.

## Tecnologias
- JavaScript
- Node.js e npm
- Cypress
- Jenkinsfile para integração contínua (presente no repositório)

## Pré-requisitos
- Node.js e npm instalados.
- Aplicação Hub de Leitura em execução e acessível pela URL configurada nos testes.

## Instalação e execução
```bash
npm install
npx cypress open
```
Execução em modo headless:
```bash
npx cypress run
```
Confira `package.json`, `cypress.config.js` e os arquivos em `cypress/` para confirmar os scripts e cenários existentes. Para gravar execuções no Cypress Cloud, configure a variável de ambiente `CYPRESS_RECORD_KEY` localmente antes de usar `npm run cy:report`; não grave chaves no código nem no repositório.

## Estrutura do projeto
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

## Desafios práticos
Preparar a aplicação alvo, selecionar elementos da interface, executar ações do usuário e validar estados visuais e funcionais sem depender de esperas arbitrárias.

## Boas práticas adotadas
- Organização dos testes em diretório próprio.
- Configuração do Cypress separada dos cenários.
- Possibilidade de integrar a execução a um pipeline.

## 📚 Aprendizados
A atividade permite praticar automação end-to-end com Cypress, desde a preparação do ambiente e seleção de elementos até a validação dos comportamentos da interface. A presença de um Jenkinsfile também oferece um ponto de partida para integrar testes ao fluxo de CI.

## Considerações finais
A URL da aplicação deve corresponder ao ambiente disponível. Consulte os arquivos de teste para identificar os cenários realmente cobertos e eventuais configurações necessárias.

---

## 🎓 Formação
Atividade desenvolvida durante a formação profissionalizante em **Quality Assurance (QA) pela EBAC — Escola Britânica de Artes Criativas e Tecnologia**.
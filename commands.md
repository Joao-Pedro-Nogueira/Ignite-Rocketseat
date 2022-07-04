# Comandos no terminal (bash) para criar projeto em React.js:

## Estrutura básica

```bash
npm init -y
npm add react
npm add react-dom
```

Estrtura no GitHub: https://github.com/Joao-Pedro-Nogueira/Ignite-Rocketseat/commit/bcb373d5b5f8d84f774a919ce7edea96414ad29c

## Configurando Babel

```bash
npm add @babel/core @babel/cli @babel/preset-env -D
```

Core = principal biblioteca do babel. 99% das funcionalidades do babel.

CLI = Executar o babel através da linha de comando (terminal).

Preset-env = Identifica qual ambiente a biblioteca está sendo executada para converter o código da melhor maneira possível.

"-D" = Dependência de desenvolvimento. Não vou utilizar nenhuma dessas bibliotecas quando o projeto for para a produção.

```bash
npx babel src/index.jsx -o dist/bundle.js
```

Cria o diretório dist/bundle.js e converte o código de entrada para um código legível para todos os browsers.

```bash
npm add @babel/preset-react -D
```

Usado para conseguir entender o código (ocm HTML) usado em React.

## Configurando Webpack

O webpack basicamente define uma série de configurações chamadas "loaders" que vão ensinar para nossa aplicação a como tratar cada tipo de arquivo importado para o projeto em React para convertê-los em arquivos "entendíveis" para o browser.

```bash
npm add webpack webpack-cli -D
```

```bash
npm add babel-loader -D
```

Biblioteca de integração entre o babel e o webpack

<!-- # Folha de Estilo

## 1. Introdução


## 2. Lint
De modo geral, lint é um programa que checa um código **estático** procurando possíveis erros comuns e de estética do código. O uso de um programa lint permite a padronização da escrita e indentação do código produzido em equipe.

## 2.1 ESLint/Preetier
ESLint é um dos programas linters utilizados para a linguagem ReactJS, enquanto o Preetier é uma extensão do VS Code que produz *warnings* relacionados à estilística do código. 

Utilizar Eslint e Preetier, em conjunto, possibilita que o *linter* faça uma checagem do código enquanto ele é escrito e ao ser salvo.

### 2.1.1 Configuração do Eslint/Prettier
Está sendo utilizado o Eslint-Airbnb, a configuração mais recomendada para React. Para utilizar Prettier em conjunto com linter é necessário especificar o plugin.

``` js
module.exports = {
  env: {
    browser: true,
    es2021: true,
  },
  extends: ["airbnb-base", "prettier"],
  parserOptions: {
    ecmaFeatures: {
      jsx: true,
    },
    ecmaVersion: 12,
    sourceType: "module",
  },
  plugins: ["prettier", "react"],
  rules: {
    "prettier/prettier": "error",
    "no-param-reassign": "off",
    "class-methods-use-this": "off"
  },
};
``` -->
# Folha de Estilo

## 1. Introdução

A folha de estilo é um documento essencial para garantir a consistência e a qualidade do código produzido em um projeto de desenvolvimento de software. Ela define diretrizes e padrões para a escrita, formatação e organização do código, contribuindo para a legibilidade, manutenibilidade e colaboração entre os membros da equipe de desenvolvimento.

## 2. Lint

De modo geral, lint é um programa que checa um código **estático** procurando possíveis erros comuns e de estética do código. O uso de um programa lint permite a padronização da escrita e indentação do código produzido em equipe.

### 2.1 ESLint/Prettier

ESLint é um dos programas linters utilizados para a linguagem ReactJS, enquanto o Prettier é uma extensão do VS Code que produz *warnings* relacionados à estilística do código.

Utilizar Eslint e Prettier, em conjunto, possibilita que o *linter* faça uma checagem do código enquanto ele é escrito e ao ser salvo.

#### 2.1.1 Configuração do Eslint/Prettier

Está sendo utilizado o Eslint-Airbnb, a configuração mais recomendada para React. Para utilizar Prettier em conjunto com linter é necessário especificar o plugin.

```js
module.exports = {
  env: {
    browser: true,
    es2021: true,
  },
  extends: ["airbnb-base", "prettier"],
  parserOptions: {
    ecmaFeatures: {
      jsx: true,
    },
    ecmaVersion: 12,
    sourceType: "module",
  },
  plugins: ["prettier", "react"],
  rules: {
    "prettier/prettier": "error",
    "no-param-reassign": "off",
    "class-methods-use-this": "off"
  },
};
```


Também é possível especificar as regras de estilística através do arquivo de configuração do Prettier.

```json
{
  "trailingComma": "es5",
  "useTabs": false,
  "tabWidth": 4,
  "semi": true,
  "singleQuote": true
}
```
Vale ressaltar que as regras especificadas manualmente podem sobrescrever as utilizadas pelo padrão Eslint-Airbnb, fugindo do padrão escolhido e do objetivo do programa linter.

## 3. Padrão de escrita e commits

Foi determinado que o código deveria seguir as regras de Conventional Commits para garantir uma melhor organização e compreensão do histórico de alterações. Conforme as regras de Conventional Commits, os commits devem seguir a estrutura:

```
<tipo>[escopo opcional]: <descrição>
```

Onde:

- <tipo>: Indica o tipo de alteração realizada. Exemplos: feat para uma nova feature, fix para uma correção de bug, docs para alterações na documentação, etc.
- [escopo opcional]: Opcionalmente, pode-se especificar o escopo da alteração.
- <descrição>: Breve descrição da alteração realizada.

***Exemplos de commits conforme as regras de Conventional Commits:***
- `feat: Adicionado componente de login`
- `fix: Corrigido erro de digitação na página de perfil`

## Referências

* [Lint. O que é isso afinal?](https://medium.com/@emerson_pereira/lint-o-que-%C3%A9-isso-afinal-83b3dc0dec59)

* [ESLint](https://eslint.org/docs/user-guide/getting-started) 

* [Prettier](https://prettier.io/docs/en/install.html)

* [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/)

### Versionamento

| Versão | Data       | Modificação          | Autor      | Revisor(es)             |
| ------ | ---------- | -------------------- | ---------- | ----------------------- |
| 1.0    | 23/04/2024 | Criação do Documento | Pedro Lima | Edvan e Philipe Serafim |
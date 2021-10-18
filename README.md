<h3 align="center">
  Template React Native
</h3>

<p align="center">Template para construção do Front End do projeto 🎓</p>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/connect-data/template-react-native?color=%2304D361">

  <a href="https://rocketseat.com.br">
    <img alt="Made by ConnectData" src="https://img.shields.io/badge/made%20by-ConnectData-%2304D361">
  </a>

  <img alt="License" src="https://img.shields.io/badge/license-MIT-%2304D361">
</p>

## :rocket: Tecnologias utilizadas

O projeto utiliza as seguintes tecnologias:

- [TypeScript](https://www.typescriptlang.org/): é um superconjunto de JavaScript que adiciona tipagem e alguns outros recursos a linguagem;
- [Expo](https://expo.io/): é uma ferramenta utilizada no desenvolvimento mobile com React Native que permite o fácil acesso às API nativas do dispositivo;
- [React Native](https://reactnative.dev/): é uma biblioteca que permite o desenvolvimento de aplicações mobile usando JavaScript e React;
- [React Native Gesture Handler](https://kmagiera.github.io/react-native-gesture-handler/) - API declarativa que permite a manipulação de toques e gestos no React Native;
- [Axios](https://github.com/axios/axios): é um cliente HTTP baseado em Promises para Browser e NodeJS;
- [Babel](https://babeljs.io/): é um compilador JavaScript gratuito e de código aberto e transpiler configurável usado no desenvolvimento de aplicações JavaScript;
- [ESLint](https://eslint.org/): é uma ferramenta de lint plugável para JavaScript e JSX;
  - [eslint-config-airbnb](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb): fornece o .eslintrc do Airbnb como uma configuração compartilhada extensível;
  - [eslint-plugin-import](https://github.com/benmosher/eslint-plugin-import): é um plugin do ESLint com regras para ajudar na validação de imports;
  - [eslint-plugin-jsx-a11y](https://github.com/evcohen/eslint-plugin-jsx-a11y): é um verificador estático AST das regras do a11y em elementos JSX;
  - [eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react): é um plugin que fornece regras de linting do ESLint específicas do React;
  - [eslint-plugin-react-hooks](https://github.com/facebook/react/tree/master/packages/eslint-plugin-react-hooks): é um plugin que fornece regras de hooks do ESLint específicas do React.
  
## :clipboard: Pré-requisitos

- [NodeJS LTS (ou superior)](https://nodejs.org/en/)
- [Expo CLI](https://docs.expo.dev/workflow/expo-cli/)

## :fire: Executando a aplicação
### :hammer_and_wrench: Configuração

#### Instalando as dependências
```
$ cd template-react-native
$ npm install
```
### :zap: Execução

#### Inicializando o projeto
```
$ expo start
```

### :iphone: Acessando a aplicação no celular de forma local
Para visualizar a aplicação no seu dispositivo móvel é necessário realizar a instalação do aplicativo Expo.
- [Android Play Store ](https://play.google.com/store/apps/details?id=host.exp.exponent) - Android Lollipop (5) e superior.
- [iOS App Store](https://itunes.com/apps/exponent) - iOS 10 e superior.

Após a instalação do aplicativo, basta realizar a leitura do QRCode gerado a partir do Metro Bundler e renderizado no seu navegador padrão.

## :open_file_folder: Estrutura de arquivos

A estrutura de arquivos está da seguinte maneira:

```bash
template-react-native
├── assets/
├── src/
│   ├── components/
│   ├── screens/
│   ├── routes/
│   ├── services/
│   ├── styles/
│   └── utils/
├── .eslintignore
├── .eslintrc.json
├── .gitignore
├── app.json
├── App.tsx
├── babel.config.js
├── package.json
├── README.md
├── tsconfig.json
└── yarn-lock.json
```
- **assets** - Diretório contendo arquivos de mídia da aplicação, que são utilizados pelas configurações do Expo;

- **src** - Diretório contendo todos os arquivos da aplicação, é criado um diretório `src` para que o código da aplicação possa ser isolado em um diretório e facilmente portado para outros projetos, se necessário;

  - **components** - Diretório onde ficam os componentes da aplicação, como forma de padronização e boas práticas. Todo componente fica dentro de um diretório com seu nome;
  
  - **screens** - Diretório que contém as telas da aplicação, como forma de padronização e boas práticas. Toda página fica dentro de um diretório com seu nome;
  
  - **routes** - Diretório onde serão criados os arquivos relacionados ao roteamento da aplicação;
  
    - **index.tsx** - Arquivo com as configurações de navegação da aplicação, nele são criados os Navigators disponibilizados na biblioteca React Navigation;

  - **services** - Diretório onde serão criados os arquivos relacionados a serviços utilizados na aplicação, por exemplo, requisições HTTP, autenticação com Firebase ou qualquer outro serviço que for utilizado;

    - **api.ts** - Arquivo com a configuração da biblioteca Axios para envio de requisições HTTP;
  
  - **styles** - Diretório onde serão criados os arquivos relacionados ao estilos globais da aplicação.
  
  - **utils** - Diretório onde serão criados os arquivos utilitários da aplicação.

- **.eslintrc.json** - Arquivo de configuração do ESLint, é nele que são inseridas as regras e configurações de Linting do projeto, tal como a configuração do Resolver para o Babel Plugin Root Import e configuração da variável global `__DEV__`;

- **App.tsx** - Arquivo raiz da aplicação, também chamado de Entry Point, é o primeiro arquivo chamado no momento do build e execução da aplicação;

- **babel.config.js** - Arquivo de configuração do Babel, é nele que é configurado o Babel Plugin Root Import para aceitar imports absolutos na aplicação usando o diretório `src` como raiz;

- **package.json** - Arquivo de configurações das dependências utilizadas no projeto;

- **tsconfig.json** - Arquivo de configuração do TypeScript no Editor, ele é o responsável por ativar o Auto Complete de códigos TypeScript na aplicação;

---

<p align="center" style="margin-top: 20px; border-top: 1px solid #eee; padding-top: 20px;">Feito com :blue_heart: por <strong> Equipe ConnectData </strong> </p>

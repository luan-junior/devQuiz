# 🧠 devQuiz

Aplicativo mobile de **quiz para desenvolvedores**, desenvolvido com **React Native e TypeScript**.

O projeto foi criado para explorar o desenvolvimento de uma aplicação mobile completa utilizando React Native, com navegação entre telas, persistência local de dados, componentes nativos e recursos de interação.

A aplicação utiliza uma arquitetura organizada por rotas e componentes, com suporte para Android e iOS.

---

## ✨ Funcionalidades

* 🧠 Quiz voltado para conhecimentos de desenvolvimento
* 📱 Aplicação mobile para Android e iOS
* 🧭 Navegação entre telas
* 💾 Persistência local de dados
* 📊 Recursos visuais para apresentação dos resultados
* ⚡ Interface desenvolvida com React Native
* 🎨 Ícones utilizando Phosphor Icons
* 📳 Feedback háptico durante a interação
* 🔊 Suporte a recursos de áudio
* 🧩 Componentização da aplicação

---

## 🛠️ Tecnologias

### Core

* **React Native 0.74.2**
* **React 18.2**
* **TypeScript 5**
* **Node.js 18+**

### Navegação

* React Navigation
* React Navigation Native Stack
* React Navigation Bottom Tabs

### Interface e interação

* React Native Gesture Handler
* React Native Reanimated
* React Native Safe Area Context
* React Native Screens
* Phosphor React Native
* React Native SVG

### Persistência

* AsyncStorage

### Recursos visuais

* React Native Skia

### Recursos adicionais

* React Native Haptic Feedback
* React Native Sound

### Qualidade

* ESLint
* Prettier
* Jest

As dependências e versões utilizadas estão definidas no `package.json` do projeto.

---

# 🏗️ Arquitetura

A aplicação possui uma estrutura baseada em **rotas, telas e componentes**, mantendo a responsabilidade de navegação separada da implementação das telas.

A entrada principal da aplicação é o `App.tsx`, que configura o `GestureHandlerRootView`, o `StatusBar` e carrega o sistema de rotas através de `src/routes`.

Estrutura principal:

```text
devQuiz/
│
├── android/
├── ios/
├── assets/
│
├── src/
│   ├── components/
│   ├── routes/
│   ├── screens/
│   └── ...
│
├── __tests__/
│
├── App.tsx
├── index.js
├── app.json
├── babel.config.js
├── metro.config.js
├── jest.config.js
├── tsconfig.json
├── .eslintrc.js
├── .prettierrc.js
├── package.json
└── README.md
```

---

# 🧭 Navegação

O projeto utiliza o **React Navigation** para controlar a navegação da aplicação.

São utilizadas duas estratégias principais:

* Native Stack Navigation
* Bottom Tab Navigation

Essa combinação permite estruturar a aplicação em diferentes fluxos e áreas de navegação.

Dependências utilizadas:

```json
{
  "@react-navigation/native": "^6.1.17",
  "@react-navigation/native-stack": "^6.9.26",
  "@react-navigation/bottom-tabs": "^6.5.20"
}
```

---

# 💾 Persistência local

O projeto utiliza o **AsyncStorage** para armazenamento local no dispositivo.

Isso permite manter informações da aplicação mesmo após o fechamento ou reinicialização do aplicativo.

```text
Aplicação
    │
    ▼
AsyncStorage
    │
    ▼
Dados persistidos
    │
    ▼
Recuperados posteriormente
```

A dependência utilizada é:

```text
@react-native-async-storage/async-storage
```

---

# 📊 Recursos visuais

O projeto utiliza o **React Native Skia** para recursos gráficos e visuais.

Essa biblioteca permite trabalhar com renderização gráfica de alto desempenho dentro do React Native.

Dependência utilizada:

```text
@shopify/react-native-skia
```

---

# 📳 Interações

Para proporcionar uma experiência mais próxima de aplicativos mobile nativos, o projeto utiliza:

### Gesture Handler

Gerenciamento de gestos e interações:

```text
react-native-gesture-handler
```

### Reanimated

Animações e interações:

```text
react-native-reanimated
```

### Haptic Feedback

Feedback tátil durante determinadas interações:

```text
react-native-haptic-feedback
```

### Sound

Recursos relacionados a áudio:

```text
react-native-sound
```

---

# 🚀 Instalação

## 📋 Pré-requisitos

Antes de executar o projeto, certifique-se de possuir o ambiente React Native configurado.

### Obrigatório

* Node.js `18+`
* npm ou Yarn
* Android Studio + Android SDK para Android
* Xcode para iOS
* CocoaPods para iOS

O projeto especifica Node.js `>=18` no `package.json`.

Para configurar o ambiente completo, consulte a documentação oficial do React Native:

[React Native — Environment Setup](https://reactnative.dev/docs/environment-setup?utm_source=chatgpt.com)

---

# 📥 Clone o projeto

```bash
git clone https://github.com/luan-junior/devQuiz.git
```

Entre no diretório:

```bash
cd devQuiz
```

---

# 📦 Instale as dependências

Utilizando npm:

```bash
npm install
```

Ou Yarn:

```bash
yarn
```

---

# ▶️ Executando o projeto

O projeto utiliza o **Metro**, bundler responsável por empacotar o código JavaScript/TypeScript da aplicação React Native.

## 1. Inicie o Metro

```bash
npm start
```

Ou:

```bash
yarn start
```

---

# 🤖 Android

Com o Metro executando, abra outro terminal e execute:

```bash
npm run android
```

Ou:

```bash
yarn android
```

O comando utiliza o React Native CLI para compilar e executar a aplicação no Android.

```text
npm run android
        │
        ▼
React Native CLI
        │
        ▼
Android Gradle
        │
        ▼
Android Emulator / Device
```

---

# 🍎 iOS

Para executar no iOS:

```bash
npm run ios
```

Ou:

```bash
yarn ios
```

Para projetos iOS, certifique-se de que o Xcode e os CocoaPods estejam configurados corretamente.

Caso necessário:

```bash
cd ios
pod install
cd ..
```

Depois:

```bash
npm run ios
```

---

# 🧪 Testes

O projeto utiliza **Jest** para testes.

Execute:

```bash
npm test
```

Ou:

```bash
yarn test
```

A configuração do Jest está presente no projeto através do `jest.config.js`.

---

# 🔍 Lint

Para verificar problemas de lint:

```bash
npm run lint
```

Ou:

```bash
yarn lint
```

O projeto utiliza ESLint com a configuração oficial do ecossistema React Native.

---

# 🎨 Formatação

O projeto utiliza **Prettier** para padronização do código.

A configuração está disponível em:

```text
.prettierrc.js
```

Para manter o código consistente, recomenda-se utilizar o Prettier durante o desenvolvimento.

---

# 📱 Plataformas

O projeto possui configuração nativa para:

| Plataforma | Suporte |
| ---------- | ------- |
| 🤖 Android | ✅       |
| 🍎 iOS     | ✅       |

As pastas `android/` e `ios/` fazem parte do repositório.

---

# 🔄 Fluxo da aplicação

O fluxo geral da aplicação pode ser representado da seguinte maneira:

```text
                 ┌───────────────┐
                 │    Usuário    │
                 └───────┬───────┘
                         │
                         ▼
                 ┌───────────────┐
                 │   React Native│
                 └───────┬───────┘
                         │
             ┌───────────┴───────────┐
             │                       │
             ▼                       ▼
      ┌─────────────┐        ┌─────────────┐
      │ Navigation  │        │ Components  │
      └──────┬──────┘        └──────┬──────┘
             │                      │
             └──────────┬───────────┘
                        │
                        ▼
                 ┌───────────────┐
                 │ Quiz / Estado │
                 └───────┬───────┘
                         │
                         ▼
                 ┌───────────────┐
                 │ AsyncStorage  │
                 └───────────────┘
```

---

# 📂 Estrutura do projeto

```text
devQuiz/
│
├── __tests__/
│
├── android/
│   └── ...
│
├── ios/
│   └── ...
│
├── assets/
│   └── ...
│
├── src/
│   ├── components/
│   │   └── ...
│   │
│   ├── routes/
│   │   └── ...
│   │
│   ├── screens/
│   │   └── ...
│   │
│   └── ...
│
├── App.tsx
├── index.js
│
├── app.json
├── babel.config.js
├── metro.config.js
├── jest.config.js
│
├── .eslintrc.js
├── .prettierrc.js
├── tsconfig.json
│
├── package.json
└── package-lock.json
```

---

# 📌 Scripts disponíveis

| Comando           | Descrição                      |
| ----------------- | ------------------------------ |
| `npm start`       | Inicia o Metro Bundler         |
| `npm run android` | Executa a aplicação no Android |
| `npm run ios`     | Executa a aplicação no iOS     |
| `npm run lint`    | Executa o ESLint               |
| `npm test`        | Executa os testes com Jest     |

Esses scripts estão definidos no `package.json`.

---

# 🎯 Objetivo do projeto

O **devQuiz** foi desenvolvido como um projeto de estudo e portfólio para explorar o desenvolvimento de aplicações mobile utilizando o ecossistema React Native.

Entre os principais conceitos trabalhados estão:

* React Native
* TypeScript
* React Navigation
* Navegação Stack
* Navegação por Tabs
* Persistência local
* AsyncStorage
* Animações
* Gesture Handler
* React Native Reanimated
* Renderização gráfica com Skia
* Feedback háptico
* Recursos de áudio
* Componentização
* Testes com Jest
* ESLint
* Prettier

---

# 🚧 Possíveis melhorias

Algumas funcionalidades que podem evoluir o projeto:

* [x] Sistema de categorias
* [x] Diferentes níveis de dificuldade
* [x] Ranking de pontuação
* [x] Histórico de partidas
* [x] Modo multiplayer
* [x] Login e perfil do usuário
* [x] Sincronização com backend
* [x] Ranking online
* [x] Novas animações
* [x] Mais efeitos sonoros
* [x] Dark/Light Mode
* [x] Testes de componentes
* [x] Testes de navegação
* [x] CI/CD para Android e iOS

---

# 👨‍💻 Autor

**Luan Junior**

Desenvolvedor Full Stack com experiência em **React, React Native, Next.js, Node.js e TypeScript**.

---

## 📄 Licença

Este projeto está disponível sob a licença definida no repositório.

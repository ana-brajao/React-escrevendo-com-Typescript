## React: escrevendo com Typescript

Sobre React, a biblioteca mais utilizada para Javascript atualmente, segundo uma pesquisa chamada State of JS, e o Typescript, uma biblioteca para tipar variáveis em Javascript.

Com essas duas bibliotecas, criaremos uma aplicação chamada "Alura Studies", na qual poderemos adicionar as tarefas que desejamos estudar e o tempo dedicado a esses estudos. Por exemplo, vou adicionar um novo estudo "React" com o tempo de 2 segundos, e outro, "Typescript", com 5 segundos.

Adicionando essas tarefas, elas vão para uma lista onde será possível selecioná-las. Selecionado "React", o tempo dessa tarefa vai diretamente para um cronômetro, que passará a mostrar "00:02". Se eu adicionar o Typescript, o valor mudará para "00:05". Depois que essa tarefa vai para o cronômetro, eu consigo inciá-la com o botão "Começar", que ativará o temporizador. Quando o tempo chegar a zero, a tarefa será completada e não será mais possível clicar sobre ela. Esse será o nosso ecossistema.

Para conseguir criar essa aplicação, primeiramente vou criar um projeto React com o create react app, além de aprender o que ele nos traz em questão de estrutura de pastas.

Também mostra a componentização, o principal que o React traz. Na aplicação, todos os elementos, como o formulário, o botão, a lista, os itens e o cronômetro, são componentes distintos. Aprenderemos a criá-los da maneira antiga, com os Class components, e de uma nova forma com os Function components.

Criando esses componentes, aprendi dois conceitos muito importantes. O primeiro deles é o DRY - Don't Repeat Yourself, ou "não se repita" em português, muito usado no React. A ideia é que não é necessário repetir códigos, já que a criação de componentes permite reaproveitá-los em outras instâncias - por exemplo, usaremos o nosso botão tanto no formulário quanto no cronômetro, alterando apenas o texto que é mostrado e o evento acionado no clique. Dessa forma, reaproveitaremos o CSS e a estrutura HTML desse botão.

Outro conceito é o chamado SRP - Single Responsibility Principle, traduzido para "Princípio da Responsabilidade Única". De forma simplificada, cada função do seu código deve ter uma responsabilidade. Em nosso caso, como o function component é uma função e um componente, cada componente deverá ter apenas uma responsabilidade. Usaremos bastante esse princípio ao criarmos nosso cronômetro.

Também usei Sass para conseguir fazer o CSS mais rápido, e Css Modules para não termos o problema de sobreposição de CSS de um componente para outro. Também aprenderemos sobre comunicação entre componentes com o Props, e sobre o estado interno de um componente com o State.

Caso você seja um veterano em React, também analisaremos como funciona uma transição/refatoração de um Class component, uma forma antiga, para um Function component, que é uma forma mais atual de se escrever React, entendendo a diferença deles, o motivo do Function component ser priorizado, entre outras coisas.

A partir de agora entraremos nessa gigantesca comunidade do React, e você entenderá por que ele é tão requisitado pelas empresas e tão adorado pelos desenvolvedores.


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

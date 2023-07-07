# React: escrevendo com Typescript (Programa Desenvolve da Boticário e Alura)

> Status do projeto: concluído

Conteúdo do curso:

* **Configurar o seu ambiente para rodar o projeto:**  <br>
Aprendemos como configurar o seu ambiente para poder criar e rodar um projeto React, instalando o Node/npm e o GIT para controlarmos as versões e/ou baixarmos a aplicação do Github.

* **Diferenciar npx de npm:** <br>
Utilizamos o npx na aplicação e aprendemos a diferenciar o comando npx do comando npm, mostrando quando é melhor usar cada um.

* **Criar um projeto com create-react-app com template typescript usando npm:** <br>
Criamos um projeto utilizando npx, entendemos que o CRA (Create React App) tem possibilidade de criar projetos com template (optamos pelo typescript), escolhendo o npm como o nosso gerenciador de pacotes padrão.

* **O Create React App estrutura o projeto:** <br>
Entendemos como o Create React App estrutura a aplicação, vendo dos arquivos de configuração (tsconfig, package.json, package-lock.json entre outros), até as pastas/arquivos que serão atualizados por nós (pasta src, arquivos app.tsx, index.tsx, index.css entre outros).

* **Funciona a pasta public:** <br>
Abordamos sobre a pasta public, para que ela serve e por que raramente mexemos nela, mostramos também o arquivo index.html e como que o React popula ele com os componentes.

* **Criar um componente com class component e como utilizá-lo:** <br>
Criamos um componente com class component, mostrando toda a sintaxe desde o extends até o retorno e o export.

* **O que é JSX:** <br>
Vimos que o React retorna na verdade um JSX, não um HTML, também falamos de algumas diferenças entre os dois.

* **Criar um function component:** <br>
Também criamos um componente com function component (a forma mais atual de se escrever componentes desde a versão 16.8), e mostramos como é mais simples criarmos dessa forma.

* **Utilizar o método map para renderizar arrays:** <br>
Renderizamos arrays de JSX com o método map, mostrando que assim conseguimos aproveitar parte do JSX e mudar apenas o valor de item para item, utilizando assim o princípio DRY (Don't Repeat Yourself).

* **Usar o CSS inline:** <br>
Aprendemos como criar o CSS inline direto no atributo, como variável JS e utilizando condicionais para mudar o estilo.

* **Utilizar CSS e Sass no projeto:** <br>
Vimos como importar CSS e SASS no projeto é fácil dentro de um projeto criado com Create React App.

* **Colocar o CSS Modules em um projeto com Create React App + Typescript:** <br>
Configuramos o projeto para aceitar CSS Modules.

* **Vantagens de se utilizar CSS Modules:** <br>
Discutimos as vantagens de se utilizar CSS Modules na aplicação.

* **Adicionar informações externas ao componente com Props:** <br>
Aprendemos a utilizar propriedades externas para reutilizar componentes de forma única.

* **Funciona o props.children:** <br>
Vimos que o React disponibiliza uma props padrão chamada children, que ao contrário das outras props, é escrita dentro do componente, abrindo e fechando a tag como em uma tag HTML.

* **O key (chaves) é importante em arrays no React:** <br>
Entendemos mais a fundo como o React trabalha com arrays, e como o key é importante para que ele não se perca entre os itens deste array.

* **Usar spread operator de forma consciente para passar props para os componentes:** <br>
Utilizamos o spread operator para poder passar todos os itens de um objeto como props para o componente, também pensamos como isso pode se tornar um problema.

* **O React utiliza os estados para atualizar os componentes:** <br>
Aprendemos como o React guarda informações que serão importantes para uma possível nova renderização de um componente.

* **Criar estados com function components e class components:** <br>
Criamos estados tanto com function components quanto com class components, entendendo como se cria esses estados em cada tipo.

* **Controlar campos de um Formulário com estados:** <br>
Aprendemos a diferença de um formulário/input controlado e não controlado, e como podemos controlá-los para pegar/mudar seus campos como quisermos.

* **Criar interfaces e reutilizá-las:** <br>
Vimos como o Typescript nos dá uma forma de criar interfaces para podermos descrever tipos mais complexos, como os props dos componentes.

* **Utilizar props e para informar uma mudança de estado:** <br>
Utilizamos a junção de props + state para podermos passar state para outros componentes e para podermos avisar que um estado deve ser mudado.

* **Compartilhar valores comuns entre componentes:** <br>
Aprendemos como criar um estado que será compartilhado entre vários componentes.

* **Extender interfaces:** <br>
Usamos a facilidade de estender uma interface dentro de outra interface para reaproveitar código.

* **Adicionar classes CSS de forma condicional:** <br>
Aprendemos a utilizar um ternário para mudar classes CSS de uma tag baseada em alguma prop com template string.

* **Criar pastas utilitárias:** <br>
Debatemos sobre formas de criar pastas com funções utilitárias compartilhadas na aplicação.

* **Funciona o ciclo de vida de um componente:** <br>
Entendemos como o ciclo de vida de um componente funciona, desde o seu nascimento até a sua morte.

* **Utilizar o useEffect:** <br>
Utilizamos o useEffect para resolver um problema que tivemos e vimos como esse hook é importante no ecossistema React.

* **Desestruturar strings:** <br>
Aprendemos que podemos desestruturar strings e que podemos colocar a opção downLevelIteration para que possamos fazer essa desestruturação.

* **Utilizar função recursiva:** <br>
Criamos uma função recursiva para resolver o problema da contagem regressiva.

* **Refatorar um class component para um function component:** <br>
Aprendemos como refatorar um class component para function component.

-----

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

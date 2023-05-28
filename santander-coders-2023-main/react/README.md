## 01. Introdução e configuração de ambiente
Vamos usar o Vite

Terminal > novo terminal

npm create vite > y > nome do projeto > selecione React > JavaScript

entre no projeto com cd

instale as dependências com npm i > npm run dev

Projeto criado.

## 02. Olá, mundo! em React

A pasta node_modules vai conter todas as dependências do projeto/React
Pasta public só tem o logo do Vite
Na pasta src vai ter o código fonte para ediar os arquivos
Arquivo gitignore para dar git

Arquivo package.json com as configurações do projeto define os dados meta, nome, privado...

Abrindo um novo terminal com npm run dev vamos executar o projeto 
Vamos deletar app.css e index.css

O arquivo main.jsx é o arquivo inicial/introdutório
Vamos apagar os imports com terminal css que apagamos para não travar o projeto

Dentro do arquivo App.jsx vamos dar nosso Hello, World com algumas linhas, quais sejam:

function App (){
    return (
        <h1>Hello, World!</h1>
        )
}

export default App

## 03. Componentes e props

Todos os componentes e funções JS estarão com letra maiúscula
É necessário exportar e importar arquivos entre módulos


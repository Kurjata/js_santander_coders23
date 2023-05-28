
<h1>Módulo 4 - JavaScript 👨‍💻</h1>
<br>

## 01. Setup: Instalação, Entrada e Saída de dados ⚙️

O JavaScript "JS" foi criado inicialmente para ser utilizado no navegador.

Inicialmente ele era consumido apenas pelo browser.

O JavaScript pode ser utilizado na integração com CSS e HTML para promover páginas interativas para o usuário.

Para esse módulo JS vamos o Node.js para que possamos programar e o interpretador/compilador converta o código em ação.

Nos é sugerido instalar as extensões 'code runner' e 'JavaScript'

Para exibir em js algo no terminal vamos usar o comand console.log("")
Para exibir um erro podemos usar console.error()
Para exibir um aviso podemos usar console.warn()

```javascript
console.log("Hello, World!")
```
<br>

## 02. Variáveis | Operadores 📁

Conceito de variáveis

Ao inserirmos um comentário, o js não lê aquela linha e aparece só para o dev como um lembrete. Utilizamos // para comentar.

Variáveis - são partes da memória que reservamos para guardar alguma informação. Geralmente chamamos uma variável através de um nome
Ex:

let idade = 26;
Para imprimir a idade utilizamos:
console.log(idade) - o resultado será 26 // criando a primeira variável

## 02.01 Tipos de variáveis 📁

Uma vez que criamos uma variável não podemos criar a mesma variável
No exemplo idade = 26, se quisermos alterar é precisa colocar:

Tipos primitivos
idade = 30;             // tipo Number

Também podemos fazer variáveis com número decimais ou textos:
let altura = 1.74          // tipo Number
let nome = "Felipe" // precisa estar entre aspas - tipo string
let estudando = true         // tipo booleano (true or false)

Sempre que precisamos imprimir mais de 1 coisa é preciso separar por vírgula

Se criarmos uma variável e não definir um valor, vai aparecer undefined (indefinida)

let null - null;            // nulo

O JS aceita criar variáveis como var. É uma variável um pouco mais antiga do JS // nao utilizar

Há variável uma variável definida como constante = const
Essa const é uma variável que não permite mudança

<br>

## 03. Operadores Aritméticos 📝

let numero1 = 20;
let numero2 = 2;

Nunca comece uma variável com número e com letra miníscula, não pode dar espaço para separar nomes compostos. O indicado é o camel case, sempre com a primeira letra minúscula e a próxima palavra maiúscula.

Operações aritiméticas básicas:

Adição : +
Subtração : -
Multiplicação : *
Divisão : /
Potência : ^
Resto da divisão : %
Exponenciação **

<br>

## 04. Operadores Booleanos ✅ or ❌

Os operadores booleanos são para comparação de verdadeiro ou falso (true or false)

Tipos de operadores:

Igualdade: == (ou ===)
Desigualdade != (ou !==)
Maior : >
Maior ou igual : >=
Menor : <
Menor ou igual : <=

CONJUNÇÕES LÓGICAS

AND => &&
OR => ||

Exemplo:

const numero = 10;

console.log(numero > 20) RESPOSTA: false

Diferença de == ou ===

Se compararmos um number com uma string do mesmo valor o JS vai aceitar pq com == ele só compara o conteúdo. Exemplo: console.log(10 == "10") A RESPOSTA SERÁ TRUE

Quando utilizamos === o JS vai comparar o conteúdo e o tipo, logo, se compararmos console.log(10 === "10") O RESULTADO SERÁ FALSE, pq o conteúdo é igual e o tipo não por ser um tipo primitivo number comparado com um string.

A recomendação é usar sempre os === para sempre fazer a comparação completa.

// Conjunções lógicas

Para consultarmos 2 variáveis juntas afim de objter uma resposta que deverá ser composta por essas duas variáveis, utilizamos o AND (&&). Exemplo:

let idade = 30;
let tenhoCNH = true;

const possorDirigir = idade >= 18 && tenhoCNH === true

console.log("Posso dirigir?", possoDirigir) A RESPOSTA SERÁ: Posso dirigir? True

tipo OR

idade = 40

const votoFacultativo = idade <18 || idade >= 70

<br>

## 05. Coerção de Tipos ⌛

Coerção Explícita (manual)

const number = 10;

console.log(numero typeof number) RESULTADO 10 number

Para fazer a conversão desse number para string e preciso:

const numero = 10

const numeroFormatoString = String(numero) - NOTE QUE A LETRA INICIAL PARA ESSA CONVERSÃO ESTÁ MAIÚSCULA

console.log(numeroFormatoString, typeof numeroFormatoString)
RESPOSTA: 10 string

console.log(Number("12345")) // transforma o number em string
console.log(parseFloat("2345.87")) // converte para float
console.log(parseInt("23443.234")) / tbm converte para float - MAS É indicado o Number
console.log(Boolean(1)) // converte para verdade
console.log(Boolean(o)) // converte para falso


O JS tem coerção implítica // faz automático

O JS não consegue fazer operações de number com string. Se tivermos a seguinte operação
console.log("10" + 1) // o JS vai transformar tudo em string e concatenar os dois. Contudo, se for uma subtração, multiplicação ou divisão, o JS converte para number e faz a conta.

<br>

## 06. Estruturas Condicionais 🛠️

A estrutura condicional também é chamada de controle de fluxo. É aquela que controla o fluxo de execução do código, ela só vai ser executada se determinada função for satisfeita.

como if

é necessário abrir parênteses. Exemplo:

const idade = 20;

if (idade >= 18) {
    console.log("Você é maior de idade!")
}

console.log("Você é menor de idade!")

// Ao executarmos isso, como o 2º console.log está fora dos conchetes, o resultado será aparecer as 2 mensagens

Para obtermos a resposta que queremos com a condiciona correta, devemos estruturar o código desta forma:

const idade = 20;

if (idade >= 18) {
    console.log("Você é maior de idade!")
} else { console.log("Você é menor de idade!")

}

Em que pese o if ser um SE o ELSE seria SE NÃO/EM CONTRA PARTIDA

<br>

## 08. Estruturas de Repetição | Laços Condicionais 🪃

O fluxo de repetição fica retornando até satisfazer sua funcionalidade.

while - repete até a condição for verdadeira até que seja verdade. Exemplo:

const input - require("readline-sync)

const numero_sorteado = 5;

const numero = input.question("Qual número você escolhe?); 
console.log() // ao fazermos isso e selecionarmos o número 3 nossa resposta será: 3 string pq o JS converte tudo em string. Para imprimir um número podemor converter o resultado com o Number e deixar assim: 

const numero - Number(input.question("Qual numero você escolhe? ));

if (numero === numero_sorteado){
    console.log("Você acertou!")
} else {
    console.log("Você errou!")
} // o problema desse código é que ao errarmos o código acaba

Para utilizarmos o while a estrutura ficará assim:

let numero = Number(input.question("Qual numero voce escolhe?" ));

while (numero !== numero_sorteado) {
    console.log("Você errou o número. Tente novamente...")

    numero = Number(input.question("Qual numero voe escolhe? ))
}

console.log("Você acertou!!!")

<br>

## 12. Funções 🔗

Função de um modo simples é um trecho do código que podemos reaproveitar, reutilizar diversas vezes.

function saudacao(){
    console.log("Olá mundo!") // não acontece nada pq só definimos a função. Precisamos definir e dpeois utilizar

}

saudacao() //agora será impresso no nosso terminal

// como enviar parâmetros para as funções?
os parênteses carregam os parâmetros

function saudacao(nome){
    console.log(Olá, ${nome}! Seja bem-vindo ao JS)
}

saudacao("Felipe")


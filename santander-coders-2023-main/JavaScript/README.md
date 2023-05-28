


##01. Setup: Instalação, Entrada e Saída de dados

O JavaScript "JS" foi criado inicialmente para ser utilizado no navegador.

Inicialmente ele era consumido apenas pelo browser.

O JavaScript pode ser utilizado na integração com CSS e HTML para promover páginas interativas para o usuário.

Para esse módulo JS vamos o Node.js para que possamos programar e o interpretador/compilador converta o código em ação.

Nos é sugerido instalar as extensões 'code runner' e 'JavaScript'

Para exibir em js algo no terminal vamos usar o comand console.log("")
Para exibir um erro podemos usar console.error()
Para exibir um aviso podemos usar console.warn()

console.log("Hello, World!")

## 02. Variáveis | Operadores

Conceito de variáveis

Ao inserirmos um comentário, o js não lê aquela linha e aparece só para o dev como um lembrete. Utilizamos // para comentar.

Variáveis - são partes da memória que reservamos para guardar alguma informação. Geralmente chamamos uma variável através de um nome
Ex:

let idade = 26;
Para imprimir a idade utilizamos:
console.log(idade) - o resultado será 26 // criando a primeira variável

## Tipos de variáveis

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

## 03. Operadores Aritméticos

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





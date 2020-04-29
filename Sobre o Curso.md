# Curso Java Script

JavaScript passo a passo.

Aqui irei mostrar todo o aprendizado de um curso realizado pela [Skylab](https://skylab.rocketseat.com.br/) para aprender JS. 

* Mas o que é o JavaScript?
* E por que procurei estudar essa linguagem? 
* Tenho que ter algum requisito para estudar?

Note que antes nunca realizei nenhum estudo voltado a área de programação. 
Assim estaremos embarcando nessa jornada do zero.

O curso é disponibilizado aborda os seguintes temas:

* JavaScript
* NodeJS
* React

#### 1 - JavaScript

JavaScript é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma. Juntamente com `HTML` e `CSS`, o `JavaScript` é uma das três principais tecnologias da World Wide Web.

#### 1.1 Introdução ao JavaScript

`$ FALAR DE JS AQUI`

    <
        FALAR SOBRE JS AQUI
    >

#### 1.2 - Estrutura do JavaScript

### Conhecendo a estrutura JavaScript


Nessa etapa vamos ter a primeira estrutura de um código JS dentro de um HTML.

Podemos observar que sempre que for utilizar o JS, temos que abrir uma tag `<script> </script>` , 
assim mostrando ao nosso código que ali realizaremos ações sejam elas apenas apresentar informações, definir variáveis, etc.

Abaixo segue um exemplo de código html com um exemplo de script.

<html>

        <script>
            console.log("Hello World") 
        </script>
        
</html>

Nesse script inserimos a função `console.log` , responsável por mostrar o retorno de uma variável ou função dentro do api console do seu
navegador web, seja chrome , firefox, etc..


>Para verificar essa função basta inspencionar sua página web e ir até a aba console.


#### 1.3 Variáveis e Dados

No JavaScript, não temos a tipagem estatica, ou seja, não precisamos definir o tipo de valor de nossa variável.

Toda váriavel no JS pode armazenar um valor diferente independente do time do script.

A variável sempre inicia por `var`, em seguida coloca o nome da variável e depois colocamos o seu valor.

<html>

        <script>
            var curso = "curso de JS";
        </script>      

</html>

*Ficar sempre atento ao `;` para indicar que a linha de codigo acabou.*

Os principais tipos de tipagem no JS são:

* **String:** *Francisco, Maria, Ana ..*
* **Inteiro:** *10 , 20 , 30 ..*
* **Decimais:** *10.2 , 5.2, 3.1 ..*
* **Booleanos:** *true , false*
* **Vetores:** [ *Francisco , Maria , Ana* ]
* **Objetos:** { *Nome: Francisco, Idade: 20, ..*}

Mostrando como fica dentro do nosso código JS:

<html>

    <script>
            var nome = "Francisco";
            var idade = 20;
            var peso = 61.2;
            var humano = true;

            var alunos = ["Francisco", "Maria", "Ana"]

            var aluno = {
                nome: "Francisco",
                idade: 20,
                peso: 61.2,
                humano: true };
    </script>

*Ficar sempre atento ao `;` para indicar que a linha de codigo acabou, e que na variável voltada a objeto, dentro de sua estrutura usamos `:`*

Ao utilizar a nossa função global  `console.log`, podemos mostrar nossa variável de acordo com nossa necessidade.

Para utilizar as variáveis em vetores ou objetos, é preciso indicar a posição de cada variável:

    >console.log("alunos[1]") → retorna o valor Maria
    >console.log(aluno.humano) → retorna o valor true

*Ficar sempre atento, no JS a primeira posição no vetor possui o index definido pelo valor `0`*



#### 1.4 Usando operções matemáticas

Para efetuar operações matemáticas, devemos criar uma váriavel de acordo com o valor que precisamos e em seguida ter uma variável para receber a operação matemática desejada.

    <script>
        var x = 10;
        var y = 20;
        var resultado = x + y;
    </script>

>**O resultado é 30**


***Dica:** Ao declarar variáveis uma em seguida da outra, podemos apenas adicionar a "virgula" para deixar nosso código mais limpo.*

    var x = 10 , y = 20;

Nesse caso podemos observar que a operação é realizada com números inteiros. Porém caso estejamos a efetuar operações matemáticas com tipagens diferentes (integer, string) o JavaScript ira concatenar os valores. Ou seja para realizar operações matemáticas devemos usar apenas com números.

    <script>
        var x = "10", y = 20;
        var resultado = x + y;
    </script>

> **O resultado é 1020**

*Podemos incrementar valores ao valor de uma variável já criada, para evitar criar muitas váriaveis. `exemplo: x = x + 2`*

#### 1.5 Funções

Em funções utilizamos a palavra `fuction` dentro do nosso script para indicar que iremos iniciar uma função em seguida do nome da função, cálculos e o retorno que deseja.

        <script>

            function soma(valor1,valor2){
                var resultado = valor1 + valor2;

                return resultado;
            }

            var resultado =soma(10,20)
          
            console.log(resultado)
        </script>

Note que sempre que indicamos a função devemos, devemos indicar qual valor queremos retornar. Para isso usamos o termo `return`.

*Ao informar uma variável na função está variável estará dispónivel apenas para a função. Para que o codigo consiga enxergar tal variável é preciso inserir a mesma ou outra novamente.*


#### 2- NodeJS

Node.js é um interpretador de JavaScript assíncrono com código aberto orientado a eventos, criado por Ryan Dahl em 2009, focado em migrar a programação do Javascript do cliente para os servidores.

#### 3- ReactJS

O React é uma biblioteca JavaScript de código aberto com foco em criar interfaces de usuário em páginas web. É mantido pelo Facebook, Instagram, outras empresas e uma comunidade de desenvolvedores individuais. É utilizado nos sites da Netflix, Imgur, Feedly, Airbnb, SeatGeek, HelloSign, Walmart e outros.

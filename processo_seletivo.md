## Resolva os exercícios a seguir 

Alguns deles estão marcados como desafio. Se não conseguir faze-los os desafios
não tem problema, você pode entregar a prova sem eles.
Caso seu código inicial já atenda o desafio vamos considerá-lo conclúido.

Você também pode deixar explicações do seu raciocínio nos comentários, 
mesmo que não chegue a uma solução do exercício.

----------------------------

#### Exercício 1a 

Crie uma função para verificar se um número é 
par ou impar e aplique-a na lista a seguir para imprimir quais
números são pares e quais são ímpares.

lista = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

function check(){
    for(let i = 0; i < lista.length; i++){
        lista[i] % 2 === 0 ? console.log(lista[i] + ' ' +  'par') : console.log(lista[i] + ' ' +  'impar')
    }
}

check()
////////////////////////////////////////////////////////////////////////////////////////////////////////////
#### Exercício 1b (desafio) 

Você consegue reduzir seu código para 1 linha?

____________________________________
///////////////////////////////////////////////////////////////////////////////////////////////////////
#### Exercício 2a: 
Escreva um algoritmo que armazene o valor 19 em uma variável A
e o valor 23 em uma variável B. A seguir troque os seus conteúdos fazendo com
que o valor que está em A passe para B e vice-versa. Ao final, escrever os 
valores que ficaram armazenados nas variáveis.

let a = 19

let b = 23

let c = a

a = b;

b = c


console.log('A:'+ a + ' ' + 'B:' +   b)

///////////////////////////////////////////////////////////////////////
#### Exercício 2b (desafio)
Repita o exercício anterior, mas seu algorítimo 
deve utilizar apenas atribuições entre a duas variáveis, sem declarar
uma terceira.


let troca = () => {

    let a = 19

    let b = 23

    if(a === 19 && b === 23)
    a = 23
   
    b = 19

    console.log('A:' + a,  'B:' + b)
}

troca()

____________________________________

#### Exercício 3a 
Crie uma função que salve os números da série de Fibonacci até chegar em x (parâmetro) interações em um array e imprima esse array.

(A série de Fibonacci é a seguinte: 0, 1, 1, 2, 3, 5, 8, 13, 21, etc... Para calculá-la, o primeiro e segundo
elementos valem 1, daí por diante, o “n-ésimo” elemento vale o (n-1)-ésimo elemento somado ao (n-2)-ésimo elemento (ex: 8 = 5 + 3))


var fibo = function (n) 
{
  if (n===1){
  
    return [0, 1];

}else{
    var s = fibo(n - 1);

    s.push(s[s.length - 1] + s[s.length - 2]);
    
    return s;
  }
};

console.log(fibo(8))

#### Exercício 3b-1 (desafio) 
Crie uma função que, recebendo o array gerado na função anterior, retorne a soma dos valores do array.

#### Exercício 3b-2 (desafio) 
Crie uma função que, recebendo o array gerado na função anterior, retorne a soma dos 
valores do array. Utilize um algoritmo diferente do desafio 3b-1. (ex: se no desáfio 3b-1 seu algorítimo usou
um loop, utilize recursão)



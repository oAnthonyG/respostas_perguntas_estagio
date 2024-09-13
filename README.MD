** Feito em JavaScript **

1) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.
R:
```function fibonacci(num) {
  let a = 0;
  let b = 1;
  let fib = b;
  while (fib < num) {
    fib = a + b;
    a = b;
    b = fib;
  }
  console.log(fib === num ? 'é um número fibonacci' : 'não é um número fibonacci')
  }
//digitar o numero desejado aqui em baixo
fibonacci(40)
```
2) Escreva um programa que verifique, em uma string, a existência da letra ‘a’, seja maiúscula ou minúscula, além de informar a quantidade de vezes em que ela ocorre.
R: 
```function contarLetrasA(string) {
  let count = 0
  for (let i = 0; i < string.length; i++) {
    if (string[i].toLowerCase() === 'a') {
      count++;
    }
  }
  console.log(`A letra A apareceu ${count } vezes`)
}
contarLetrasA('Pastel de Banana com Ameixa')
```
3) Observe o trecho de código abaixo: int INDICE = 12, SOMA = 0, K = 1; enquanto K < INDICE faça { K = K + 1; SOMA = SOMA + K; } imprimir(SOMA);
R: 
```const indice = 12
let k = 1
let soma = 0
while(k < indice){
  k = k + 1
  soma = soma + k
}
console.log(soma)
// resposta é 77
```
4) Descubra a lógica e complete o próximo elemento:
a) 1, 3, 5, 7, 9
b) 2, 4, 8, 16, 32, 64, 128
c) 0, 1, 4, 9, 16, 25, 36, 49
d) 4, 16, 36, 64, 100
e) 1, 1, 2, 3, 5, 8, 13
f) 2,10, 12, 16, 17, 18, 19, 20

5) Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em salas diferentes. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada. Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?

R: Ligaria o primeiro interruptor e deixaria por alguns minutos até a lampada ficar quente e desligaria, depois ligaria o segundo interruptor e iria andando até a lampada que tinha ligado que vai estar apagada porem quente, e assim o calor indicaria que a lampada esteve ligada e depois foi desligada.
Sabendo qual interruptor da Lampada acessa e da apagada porem quente, sobra o terceiro interruptor que é da lampada fria e apagada.

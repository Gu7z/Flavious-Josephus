# Flavious-Josephus
Resolvendo o problema lógico de Flavious Josephus.
Os inputs devem ser no formato:
Linha 1: Quantidade de casos
Linha 2 em diante: Casos (Quantidade de homens e quantidade de saltos, respectivamente)
Ex: 
* 3
* 5 2 
* 6 3
* 1234 233

#### Texto retirado do site Uri Online
O problema de Josephus é assim conhecido por causa da lenda de Flavius Josephus, um historiador judeu que viveu no século 1. Segundo o relato de Josephus do cerco de Yodfat, ele e seus companheiros (40 soldados) foram presos em uma caverna, cuja saída foi bloqueada pelos romanos. Eles preferiram suicidar-se a serem capturados, e decidiram que iriam formar um círculo e começar a matar-se pulando de três em três. Josephus afirma que, por sorte ou talvez pela mão de Deus, ele permaneceu por último e preferiu entregar-se aos romanos a suicidar-se.

#### Explicação de funcionamento da lógica
Temos 3 váriaveis de controle e um array.
As tres vars são ``` contador ```, ``` volta ```, ``` num ``` e o array é ``` homens ```

A variavel num é a que recebe os saltos.

O array homens é o controlador, um array de true or false:
* caso false os homens ainda estão "vivos" (false para morreram);
* caso true os homens "morreram" (true para morreram).

A variavel volta, aumenta até o tamanho do array ```homens```:
* Serve para controlar a posição que estamos verificando;
* Mudamos o true or false na posição que volta estiver.
 
A variavel contador, aumenta "infinitamente":
* Serve para verificar se estamos no salto correto para mudar o true ou false

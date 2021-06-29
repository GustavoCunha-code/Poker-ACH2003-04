# Poker-ACH2003-04

Exercício de Computação Orientada a Objeto da turma ACH2003-04, ministrada pelo Professor Marcelo Chaim.<br>

## Instruções e Observações

Sintam-se livres para editar e adicionar qualquer classe e método que acharem necessário.<br>

Os métodos que devem ser criados estão na parte de "Issues". Nessas Issues, tem comentários com sugesões de implementação, mas vocês não precisam seguí-las, vocês estão livres para implementar esse programa do jeito que quiserem.

MAS É IMPORTANTE EXPLICAR O FUNCIONAMENTO DOS MÉTODOS ATRAVÉS DE COMENTÁRIOS E DA DOCUMENTAÇÃO.

OBS: Escrever uma boa documentação no README conta como contribuição ;)
Então não deixem de registrar como o programa funciona.

No final desse README tem uma sessão "Contribuidores" para vocês se registrarem.

## Explicação das classes

### Card

Carta possui dois atributos: seu valor (rank) e seu naipe (suit). Esta classe possui getters e setters para que possa ser possível acessar e alterar os valores dos atributos e o toString que foi sobrescrito para que para que em todas as situações onde será necessário converter o objeto para uma String ele será chamado para realizar tal função, onde na qual foi utilizada aspas duplas para indicar para que o compilar já entenda que logo em seguida acontecerá uma concatenação de strings.	return "" + this.rank + this.suit; Ainda possui um método compareCard(Card other), onde irá comparar a carta que o chamou com a outra carta que foi passada como parametro.

### Player

Jogador possui dois atributos: Array de Cards e um valor indicando o quão alta sua mão é.
No seu contrutor, recebe uma String que á a mão de entrada e este irá chamar o split para retirar os espaços entre as cartas e assim armazenar dentro de um array de Strings. A quantidade de cartas recebida pelo jogador irá corresponder ao tamanho do array de Cards. A cada posição do array de cartas será alocado um objeto do tipo carta. Como padrão foi definido que o index é zero. Ainda teremos getters e setters para além de um toString() para representar todas as cartas que estão na mão do jogador. 

### Table

Possui três atributos:

- Array de Players
- Valor inteiro highHandIndex (este é o responsável por indicar qual a posição da mão mais alta).
- Array final de Strings da Classe hands com a sequência ordenada do maior para o menor das possíveis mãos do poker

Os métodos são:

- defineHand chama os métodos que identificam cada uma das mãos do poker
- isRoyalFlush, isStraightFlush, isFourKind, isFullHouse, isFlush, isStraight, isThreeKind, isTwoPair, isPair
- individualTest imprime as 5 cartas testadas e a sua respectiva classificação
- sortCards é o método que ordena da maior carta para a menor carta. Ela utiliza o algoritmo Quicksort. Para isso ela utiliza os métodos:
  - Quicksort, trocaValorEntreCards, particiona. 

Obs.: Em termos de análise de complexidade assintótica a implementação dos métodos e a ordem na qual eles são chamados podem influenciar no desempenho do código, pois para a verificação de alguns casos há uma certa repetição de checagem em relação aos demais. 

## Contribuidores

<b> Escreva aqui seu nome, NUSP e usuário do Github </b>

- Felipe Furquim - 11208030 - FvFurquim
- Fábio Yamada - 5690619 - fabioheiji
- Silas Bovolin Reis  - 11796739 - SilasReisUSP
- Felipe Oliveira - 11925242 - felipeoes
- Gustavo Cunha - 10438400 - GustavoCunha-code

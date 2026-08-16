#linguagens-de-programação #backend 

# O que é programação assíncrona e síncrona?
A programação síncrona e assíncrona são duas abordagens distintas para lidar com operações em um programa ou sistema de software. Cada uma tem suas próprias características e é adequada para diferentes cenários de desenvolvimento.

![[Pasted image 20260606151408.png]]

## Como funciona a programação síncrona?
Na programação síncrona, as operações são executadas em sequência, uma após a outra, de forma bloqueante. Cada operação espera a operação anterior ser concluída antes de prosseguir.

## Como funciona a programação assíncrona?
Na programação assíncrona, as operações são iniciadas de forma independente e não bloqueante. O programa pode continuar executando outras operações enquanto aguarda o resultado das operações assíncronas. Geralmente utiliza callbacks, promises ou async/await para lidar com a conclusãO das operações assíncronas.

![[Pasted image 20260606151805.png]]

## Quando devemos utilizar a comunicação síncrona?
A comunicação síncrona, é ideal para situações em que a obtenção de dados é direta, o processamento é rápido e a simplicidade é valorizada.

## Quando devemos utilizar a comunicação assíncrona?
A comunicação assíncrona é mais apropriada em situações onde a eficiência e a capacidade de resposta são fundamentais, especialmente em operações que envolvem I/O (entrada/saída) intensivo, como acesso a banco de dados, chamada de API, operações de rede e interações com sistemas externos.


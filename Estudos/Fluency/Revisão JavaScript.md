#linguagens-de-programação #backend 

# Tipos de dados em JavaScript
- Números: em JavaScript todos os números são implementados em double-precision 64-bit binary format IEEE 754 (Por exemplo, um número entre -(253 a 1) e (253 a 1)). Não havendo especificação de tipo integer, além de ser capaz de representar números de ponto flutuante, o tipo de número tem três valores simbólicos: +Infinity, -Infinity e um NaN (not-a-number).
- Texto: o tipo String do JavaScript é usado para representar informações de texto. É um conjunto de 'elementos' composto por valores inteiros de 16-bits sem sinal. Cada elemento dentro da String ocupa uma posição dentro dessa String. O primeiro elemento está no índice 0, o próximo no índice 1, e assim sucessivamente. O tamanho de uma String é a quantidade de elementos que ela possui.
- Booleans: em JavaScript, um boolean é um tipo de dado que pode ter dois valores: true ou false. É usado para representar valores de verdade, sendo fundamental em operações lógicas e controle de fluxo de código.

# Declaração de variáveis
Em JavaScript uma variável é um contêiner que armazena dados. Ela permite que você possa facilmente utilizar e manipular esse valor ao longo do seu código. Variáveis são fundamentais para a programação, pois facilitam o gerenciamento de dados dinâmicos e a criação de programas flexíveis.

Em JavaScript ==var==, ==let== e ==const== são usadas para declarar variáveis, mas têm diferenças importantes em termos de escopo, redeclaração, reatribuição e hoisting. Suas principais diferenças são:
- ==var==: Escopo de função, permite redeclaração e reatribuiçãO, sofre hoisting com inicialização como undefined.
- ==let==: Escopo de bloco, não permite redeclaração no mesmo escopo, permite reatribuição, sofre hoisting mas não é inicializado.
- ==const==: Escopo de bloco, não permite redeclaração nem reatribuição, sofre hoisting mas não é inicializado, valor imutável, mas objetos e arrays podem ter suas propriedades e elementos modificados.

# Uso de operadores
Em JavaScript, operadores são símbolos especiais que são usados para realizar operações em operandos (valores ou variáveis). Eles podem ser classificados em várias categorias, incluindo operadores aritméticos, de atribuição, de comparação, lógicos, bit a bit, de string e mais.

## Operadores de atribuição

```JavaScript  
	let x = 10; //Atribuição simples, X recebe 10
	x += 5; // Adiciona 5 ao valor original de X, totalizando 15
	x -= 3; //Remove 3 do valor original de X, totalizando 12
	x *= 2; //Multiplica o valor original de X por 2, totalizando 24
	x %= 4; //Divide o valor de x por 4 e guarda o resto da divisão
```
## Operadores aritméticos

```JavaScript  
	let a = 5;
	let b = 3;
	
	let soma = a + b; 
	let subtracao = a - b; 
	let multiplicacao = a * b;
	let divisao = a / b;
	let resto_divisao = a % b;
	let exponencial = a ** b;
	
	// incremento (++)
	let c = 5;
	c++;// Aumenta o valor de c em 1
	
	// decremento (--)
	let d = 5;
	d--;//Diminui o valor de d em 1
```

## Operadores de Comparação

```JavaScript  
	let igual = (5 == '5');//true
	let exatamente_igual = (5 === '5');//false
	let diferente = (5 != '5');//false
	let totalmente_diferente = (5 !== '5');//true
	let maior = (5  > 3);//true
	let maior_igual = (5  >= 5);//true
	let menor = (3 < 5);//true
	let menor_igual = (3 <= 3);//true
```

## Operadores Lógicos

```JavaScript  
	let e = (true && true);//true
	let ou = (true || false);//false
	let nao = (!true);//false
```

## Operadores de String

```JavaScript  
	let message = 'Olá, '+'mundo';//'Olá, mundo'
	let mensagem = 'Olá';
	mensagem += ', mundo';//'Olá, mundo'
```

## Operadores Unários

```JavaScript  
	typeof 4.5;//Returna number
	typeof 'Olá';//Returna string
	typeof NaN;//Returna number
	typeof Infinity;//Returna number
```
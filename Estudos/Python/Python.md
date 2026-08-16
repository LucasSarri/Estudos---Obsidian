#linguagens-de-programação #python 

* Linguagem de Alto Nível
	  É uma linguagem que se aproxima mais da linguagem humana do que da linguagem de máquina.
* Interpretada
	  O código é executado diretamente pelo interpretador, sem a necessidade de compilar o mesmo para transformá-lo em linguagem de máquina.
* Orientada a Objetos
	  A linguagem na verdade é multi paradigma, ela suporta vários tipos de paradigmas da programação. 


Quando for criar arquivos de **script**, como boa prática o arquivo principal é chamado de **main** e todos são salvos com a extensão **.py**. Para executar um **script** basta acessar o diretório que o mesmo se encontra com o **cmd**, e digitar:

```terminal
python nomeArquivo.py
```
***
# Variáveis
O papel de uma variável é armazenar dados, existem os seguintes tipos de variáveis:
* **int**: variáveis do tipo **int** armazenam números inteiros, como uma idade.
```python
idade = 33
```
* **str**: variáveis do tipo **str** ou **string** armazenam texto, como um nome.
```python
nome = "Gabriel"
```
* **float**: variáveis do tipo float armazenam números decimais, como altura.
```python
altura = 1.75
```
* **boolean**: variáveis do tipo **boolean** armazenam estados lógicos, sendo verdadeiro ou falso. É possível também armazenar condições.
```python
# armazenando estados lógicos
is_python = True
is_java = False
# armazenando condições
ingressos = 50
compradores = 250
tem_ingresso_suficiente = (ingressos >= compradores)
```
***
# Comandos
## Print
O comando **print()** é utilizado para apresentar uma determinada informação no terminal, seguem alguns exemplos:
```python
print("oi") -> oi
print(1+1) -> 2
print(10/2) -> 5
```
## Input
O comando **input()** é utilizado para armazenar a entrada de dados do usuário, seguem alguns exemplos:
```python
nome = input("Digite seu nome:")
idade = input("Digite sua idade:")
peso = input("Digite seu peso:")
```
**OBS**: é importante ter em mente que o comando **input** armazena os dados como **string**.
## Int
O comando **int()** é utilizado para converter um dado do tipo **string** para o tipo **int**, seguem alguns exemplos:
```python
# fazendo de forma mais ilustrativa
idadeEmString = input("Digite sua idade:")
idadeEmInt = int(idadeEmString)
# fazendo de forma direta
idade = int(input("Digite sua idade:"))
```
## Float
O comando **float()** é utilizado para converter um dado do tipo **string** para o tipo **float**, seguem alguns exemplos:
```python
# fazendo de forma mais ilustrativa
pesoEmString = input("Digite seu peso:")
pesoEmFloat = float(idadeEmpeso)
# fazendo de forma direta
idade = float(input("Digite seu peso:"))
```
## Type
O comando **type()** é utilizado para identificar o tipo de alguma variável, seguem alguns exemplos:
```python
# criação das variáveis
nome = input("Digite seu nome:")
idade = int(input("Digite sua idade:"))
peso = float(input("Digite seu peso:"))
# apresentando os tipos das variáveis
print(type(nome))
print(type(idade))
print(type(peso))
```
***
# Operadores








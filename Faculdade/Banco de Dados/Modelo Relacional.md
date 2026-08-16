#banco_de_dados

É um dos [[Modelos de Dados|modelos de dados]] mais utilizados utilizados atualmente, suas primeiras implementações comerciais se tornaram disponíveis no início da década de 1980. Foi implantado em uma grande quantidade de sistemas comerciais.

Representa o [[Bancos de Dados|banco de dados]] como uma coleção de **relações** entre **tabelas** de valores. Onde uma **Tabela** é formada por:
* Linha: representa uma coleção de valores de **dados** relacionados. Um fato que normalmente corresponde a uma entidade ou relacionamento do mundo real.
* Coluna: cada coluna corresponde a um atributo da entidade dentro da **tabela**.

# Restrições
As restrições definem o que é permitido dentro do banco de dados, existem os seguintes tipos:
* Restrições inerentes ao [[Modelos de Dados|modelo de dados]].
* Restrições baseadas em [[Esquemas|esquemas]]: podem ser expressas diretamente nos [[Esquemas|esquemas]] do [[Modelos de Dados|modelo de dados]].
* Restrições baseadas na aplicação: não podem ser diretamente expressas nos [[Esquemas|esquemas]], por isso são expressas e impostas pelos programas de aplicação.
* Restrições de domínio: são as delimitações dos tipos e formato dos **dados** que podem ser aceitos, além do intervalo e conjunto de valores que podem ser aceitos.
* Restrições de chave: 
	* Duas linhas não podem ter a mesma combinação de valores para todos seus atributos

# Superchave
É um subconjunto do [[Bancos de Dados|banco de dados]], que possui os atributos para identificar de maneira única uma tupla.

# Chave
É um subconjunto de uma [[Modelo Relacional#Superchave|Superchave]], que possa identificar uma tupla de maneira única com o mínimo de componentes possível.

## Chave Candidata
Um esquema de relação pode ter mais de uma [[Modelo Relacional#Chave|chave]], as [[Modelo Relacional#Chave Candidata|chave candidata]] são alternativas para serem [[Modelo Relacional#Chave Primária|chaves primárias]].

# Chave Primária
É um atributo específico selecionado para identificar uma relação
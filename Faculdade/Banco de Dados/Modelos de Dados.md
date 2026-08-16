#banco_de_dados

Uma coleção de conceitos para descrever a estrutura de um [[Bancos de Dados|banco de dados]], oferecendo os meios necessários para alcançar a [[Abstração de Dados|abstração de dados]].

# Operações Básicas
Especifica o funcionamento das funções básicas de um [[Bancos de Dados|banco de dados]], como recuperações e atualizações no mesmo.

# Modelos de dados de alto nível ou conceituais
Estes modelos são próximos a forma que os usuários percebem os **dados**.

## Modelo Entidade-Relacionamento
Este modelo possuí uma série de elementos que apresentam de forma simplificada o funcionamento de um [[Bancos de Dados|banco de dados]]. É composto pelos elementos:

### Entidade
Representa um objeto ou conceito do mundo real no modelo
 
 #### Atributo
 Representa uma propriedade dentro de uma entidade, é utilizado para descrever melhor uma entidade.
 
### Relacionamento
Basicamente representa a associação entre as entidades

# Modelos de dados de baixo nível ou físicos
Estes modelos descrevem de forma detalhada como os **dados** são armazenados no computador.

## Caminho de acesso
Estrutura que torna mais eficiente a busca por registros de um [[Bancos de Dados|banco de dados]] em particular

### Índice
O índice é um exemplo de [[Modelos de Dados#Caminho de acesso|caminho de acesso]], que permite o acesso direto aos **dados** usando um termo de índice ou uma palavra-chave.

# Modelos de dados representativos
Estes possuem conceitos facilmente entendidos pelos usuários finais, mas também são similares ao modo que os **dados** são armazenados e organizados no computador.

## Modelo de dados relacional
Esse modelo é usado com mais frequência nos [[SBGD|SGBDs]] comerciais tradicionais

## Modelo de dados de objeto
Um modelo de **dados** de implementação de nível mais alto e próximo aos [[Modelos de Dados#Modelos de dados de alto nível ou conceituais|modelos de dados conceituais]].
#banco_de_dados

Um **sistema gerenciador de banco de dados** (**SGBD**), basicamente é uma coleção de programas que permite aos usuários criar e manter um ou mais [[Bancos de Dados|bancos de dados]].

Os **SGBD** são utilizados na manipulação de [[Bancos de Dados|bancos de dados]], permitindo aos usuário consultarem, atualizarem, removerem e inserirem informações nos mesmos. 

# Vantagens de um SGBD
Ao utilizar um **SGBD** existem as seguintes vantagens:
* Controlam a redundância, utilizando a **Normalização** e **Desnormalização**, as vezes é necessário usar a **redundância controlada** para melhorar o desempenho das consultas.
* Restrição de acesso não autorizado, possuí um **subsistema** de segurança e autorização.
* Podem oferecer **armazenamento persistente** para objetos do programa, como um **objeto** complexo em *C++* pode ser armazenado de forma persistente em um **SGBD** orientado a objeto.
* Problema de divergência de impedância, os [[Bancos de Dados|sistemas de banco de dados]] orientados a **objeto** em geral oferecem compatibilidade da **estrutura de dados**.
* Oferece **estruturas de armazenamento** e **técnicas de pesquisa** para o processamento eficiente de uma consulta, como [[Índices|índices]], [[Buffering|buffering]] ou [[Caching|caching]], e por fim o processamento e otimização de consulta.
* Oferecem **backup** e recuperação, possuem um **subsistema de backup e recuperação** que é responsável por fazer essas operações.
* Oferecem múltiplas interfaces de usuário, Interfaces gráficas do usuário (**GUI**s).
* Representando relacionamentos complexos entre **dados**, pode incluir muitas variedades de **dados** que estão inter-relacionados de diversas maneiras.
* Impondo **restrições de integridade**, podendo impor as restrições **referencial** e de **chave**.

# Linguagens do **SGBD**
## Linguagem de definição de dados (DDL)
Define

## Linguagem de definição de armazenamento (SDL)
Especifica o [[Esquemas|esquema interno]]

## Linguagem de definição de visão (VDL)
Especifica **visões do usuário** e seus mapeamentos ao [[Esquemas|esquema conceitual]]

## Linguagem de manipulação de **dados** (DML)
Uma linguagem que inclui a recuperação, inserção, exclusão e modificação dos **dados**.

### DML de alto nível ou não procedural
Pode ser utilizada para especificar operações de [[Bancos de Dados|banco dedados]] complexas de forma concisa, pode trabalhar com um conjunto de cada vez ou orientadas a conjuntos.

### DML de baixo nível ou procedural
Deve ser embutida em uma linguagem de programação de uso geral, trabalha com um registro de cada vez.

# Interfaces de **SGBD**
* Interfaces baseadas em menu para clientes Web ou navegação.
* Interfaces baseadas em formulário
* Interfaces gráficas com o usuário
* Interfaces de linguagem natural
* Entrada e saída de voz
* Interfaces para usuários paramétricos
* Interfaces para [[Atores em cena#Administrador de Banco de Dados (**DBA**)|DBA]]

# Módulos componentes do **SGBD**
* Gerenciamento de buffer
* Gerenciador de **dados** armazenados
* Compilador da [[SBGD#Linguagem de definição de dados (DDL)|DDL]]
* Interface de consulta interativa
	* Compilador de consulta
	* Otimizador de consulta
* Pré-compilador
* Processador de [[Bancos de Dados|banco de dados]] em tempo de execução
* [[Catálogo]] do sistema
* Sistema de controle de concorrência
* Sistema de backup e recuperação
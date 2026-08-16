#banco_de_dados

Um [[Bancos de Dados|banco de dados]], basicamente é uma **coleção de dados** relacionados, fatos conhecidos que podem ser registrados e possuem um significado implícito.

Para se gerenciar um [[Bancos de Dados|banco de dados]] são utilizados os [[SBGD|SGBD's]], onde é possível gerenciar a estrutura dele, os tipos e restrições dos **dados** que serão armazenados.

# Fases de um projeto de **Banco de Dados**
* Especificação e análise de requisitos
* Projeto conceitual
* Projeto lógico
* Projeto físico

# Características de um **Banco de Dados**
Quando se utiliza um [[Bancos de Dados|banco de dados]], este atua como repositório centralizado que armazena os **dados** que podem ser acessados por diversos usuários

Um [[Bancos de Dados|banco de dados]] possuí uma natureza de autodescrição, ou seja, o sistema de [[Bancos de Dados|banco de dados]] contém a definição completa de sua estrutura e restrições. Sua estrutura é descrita através dos [[Metadados|metadados]] utilizando um [[Catálogo|catálogo]].

O isolamento entre os programas e os **dados** ocorre pelo fato da estrutura dos arquivos dos **dados** ser armazenada no [[Catálogo|catálogo]] pelo [[SBGD]] separadamente dos programas de acesso. E a independência da operação do programa ocorre pois a **interface** de uma operação inclui o nome da operação e os tipos de **dados** de seus argumentos e a implementação da operação pode ser alterada livremente sem afetar a **interface**.

A  [[Abstração de Dados|abstração de dados]] permite que ocorra a independência de **dados** do programa e a independência da operação do sistema. Ela pode ocorrer de duas formas:
	* Representação conceitual de **dados**: Não inclui muitos dos detalhes como os **dados** são armazenados ou como as operações são implementadas.
	* [[Modelos de Dados|Modelo de dados]]: é uma forma de oferecer representação conceitual.

Um [[Bancos de Dados|banco de dados]] possui suporte para múltiplas **visões dos dados**,  uma **visão** é um subconjunto do [[Bancos de Dados|banco de dados]] que contém **dados virtuais** derivados dos arquivos do mesmo, mas que não estão armazenados explicitamente.

É permitido que múltiplos usuários acessem ele ao mesmo tempo, o **software de controle de concorrência** garante que estes vários usuários tentando atualizar o mesmo **dado** façam isso de forma controlada. Esse *software* utiliza [[Transações|transações]] curtas de operações básicas (inserções e atualizações) e poucas leituras, as operações costumam envolver poucos registros, mas podem haver milhares de [[Transações|transações]] concorrentes.

# Utilitários de um **Banco de Dados**
* Carga: carrega os arquivos de **dados** existentes.
* Backup: cria uma cópia de segurança do [[Bancos de Dados|banco de dados]].
* Reorganização do armazenamento do [[Bancos de Dados|banco de dados]]: reorganiza um conjunto de arquivos do [[Bancos de Dados|banco de dados]] em diferentes organizações de arquivo.
* Monitoração de desempenho: monitora o uso do [[Bancos de Dados|banco de dados]] e oferece as estatísticas ao [[Atores em cena#Administrador de Banco de Dados (**DBA**)|DBA]].

# História das aplicações de **Banco de Dados**
Antigas aplicações de [[Bancos de Dados|banco de dados]] nos anos de (1960 e 1970) seguiam os modelos **hierárquicos** e **de rede**.  Nestes modelos existiam as seguintes características:
* Grande quantidade de **registros** com estrutura semelhante.
* Misturavam relacionamento conceitual e armazenamento físico de **dados**.
* Sem flexibilidade para armazenar **dados**.
* Perda de desempenho para atender consulta não previstas inicialmente no **modelo de dados**.

O modelo relacional começou a ser usado no final dos anos 70 e no início dos anos 80, e se tornaram a tecnologia mais popular de [[Bancos de Dados|banco de dados]] comerciais, que possuem as seguintes características:
* Separa o armazenamento físico dos **dados** de sua **representação conceitual**.
* Fornece uma base matemática para a representação e consulta dos **dados**.

Com o surgimento das aplicações orientadas a **objeto** começou a existir a necessidade de [[Bancos de Dados|bancos de dados]] mais complexos, que surgiram 1990 e são usados principalmente em aplicações especializadas.










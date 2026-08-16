#banco_de_dados

Uma **transação** trata-se de uma sequência de operações no [[Bancos de Dados|banco de dados]], que pode fazer que alguns **dados** sejam lidos e outros sejam gravados.

Uma **transação** segue as propriedades **ACID**, que são: 
* As transações devem manter a consistência dos **dados** de um [[Bancos de Dados|banco de dados]].
* **Propriedade da Atomicidade**, todas as operações da transação são executadas ou nenhuma é.
* **Propriedade da Consistência**, o [[Bancos de Dados|banco de dados]] deve estar em um estado consistente após a execução da transação.
* **Propriedade de Isolamento**, cada transação parece executar isoladamente das outras transações, mesmo em paralelo.
* **Propriedade de Duração**, após o *commit* da transação, todas as atualizações do [[Bancos de Dados|banco de dados]] devem ser salvas, ainda que haja alguma falha no sistema e os **dados** ainda não foram escritos em **disco**
#linguagens-de-programação #backend 

# Relembrando o conceito de API
Uma API promove a conexão entre um usuário e uma aplicação, mas sem que ele precise dos detalhes da estrutura e do desenvolvimento do sistema que se está tentando utilizar. Isso somente é possível utilizando um conjunto de definições e protocolos usados no desenvolvimento e na integração de software e de aplicações.

# O que faz uma API ser do tipo REST?
Uma API do tipo REST (Representational State Transfer) segue um conjunto específico de princípios e restrições projetados para criar sistemas distribuídos escaláveis e eficientes na web. Uma REST indica então um conjunto de restrições que devem ser seguidas no desenvolvimento de uma aplicação na internet.

# Princípios fundamentais de uma API RESTful
- Arquitetura Cliente-Servidor: o cliente (que pode ser um navegador, um aplicativo móvel, etc) e o servidor (onde a lógica e os dados estão armazenados) são separados, permitindo que ambos evoluam de forma independente.
- Stateless (Sem estado): Cada requisição do cliente para o servidor deve conter todas as informações necessárias para entender e processar o pedido. O servidor não deve armazenar nenhuma informação sobre o estado do cliente entre as requisições. Isso simplifica a escalabilidade e a recuperação de falhas.
- Cacheabilidade: As respostas das requisições devem ser explicitamente marcadas como cacheáveis ou não-cacheáveis. Se uma resposta é cacheável, o cliente pode reutilizá-la para requisições futuras, melhorando a eficiência e a performance.
- Interface uniforme:
	- Recursos são identificados em requisições usando URIs (Uniform Resource Identifiers)
	- Clientes interagem com os recursos usando suas representações (ex: JSON ou XML)
	- Cada mensagem contém informações suficientes para descrever como processar a mensagem (ex: enviar informações utilizando cabeçalhos HTTP).
	- O cliente interage com a aplicação inteiramente através de hiperlinks fornecidos dinamicamente pela aplicação.

# Como funcionam as APIs REST?
- URIs: Utiliza URI para identificar recursos de forma clara e consistente. EX: http://api.exemplo.com/usuarios/123, poderia referir-se ao usuário com ID 123.
- Métodos HTTP: Utiliza métodos HTTP (GET, POST, PUT, DELETE, etc) para realizar operações CRUD (Create, Read, Update, Delete) em recursos.
- Formato de dados: As respostas geralmente são em formatos de dados padronizados como JSON ou XML.

![[Pasted image 20260604165227.png]]
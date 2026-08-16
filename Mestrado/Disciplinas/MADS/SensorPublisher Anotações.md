#MADS

# Introdução
A Internet das Coisas (IoT) revolucionou a coleta de dados em diversas áreas e trouxe uma mudança de paradigma nas geociências modernas.

Oceanografia, estudos de mobilidade e ciências ambientais são apenas algumas das áreas que utilizam sistemas que combinam IoT e dados geográficos. Ao empregar sensores especializados, coleta de dados em tempo real, essas tecnologias oferecem insights valiosos sobre fenômenos complexos.

Desenvolver dashboards de IoT que explorem os dados coletados é um desafio significativo para pesquisadores em geociências. Isso envolve gerenciar formatos de dados complexos, compreender tecnologias avançadas de sistemas de informação e desenvolver funcionalidades para visualização e interpretação de dados.

Embora cada dashboard de IoT seja diferente dos demais, todos compartilham várias características em comum, como:
1. Utiliza um mecanismo de ingestão de dados orientado a fluxo (stream) para coletar dados provenientes dos sensores.
2. Ser baseado em um data lake, devido à heterogeneidade dos dados.
3. Fornecer ferramentas para descoberta e exploração das informações, permitindo determinar se os conjuntos de dados são revelantes e apropriados.
4. Oferecer um conjunto de ferramentas de processamento para trabalhar com os dados armazenados no data lake e gerar novas informações.
5. Permitir a interação com o sistema por meio de ferramentas baseadas em Sistemas de Informação Geográfica (SIG/GIS) para visualizar informações e resultados em mapas, além de listagens tradicionais.

Apesar das variações existentes entre os sistemas, a presença dessas características compartilhadas sugere que eles podem ser gerenciados como uma família de produtos de software, potencialmente usando técnicas de gerenciamento de variabilidade.

Neste artigo, é descrito um framework que cria sistemas de informação baseados na web e em sensores, com foco em armazenamento e análise de dados (data warehousing). As contribuições concentram-se em três áreas principais:
- Uma linha de produtos de software (Software Product Line): descrevemos uma SPL projetada especificamente para sistemas de informação que coletam e visualizam dados provenientes de redes de sensores.
- Uma linguagem específica de domínio (Domain-Specific Language - DSL): é proposto uma DSL para definir e trabalhar com medições de sensores e suas propriedades. Essa DSL é uma ferramenta útil para especialistas do domínio que não têm familiaridade com desenvolvimento de código.
- Uma ferramenta de desenvolvimento low-code: propomos uma ferramenta que pode ser utilizada via linha de comando ou por meio de um navegador web para criar e implantar sistemas de informação complexos baseados em sensores.

# Um framework para criação de dashboards de IoT
O framework consiste em um fluxo de trabalho automatizado que ajuda pesquisadores de geociências a permanecerem focados no problema do domínio, as etapas do fluxo de trabalho do framework são as seguintes:
1. Descrição do produto (Product Description): Os usuários começam definindo o modelo de dados dos sensores utilizando uma DSL (linguagem específica de domínio). Eles também especificam as funcionalidades desejadas do produto e as preferências de implementação (deploy).
2. Sensor publisher: este é o componente central do framework, responsável por orquestrar todo o fluxo de trabalho. Ele verifica se a definiçãO do sensor fornecida pelo usuário está correta e confirma se a seleção de funcionalidades é uma configuração válida de acordo com as restrições do modelo de features. Uma vez validado, ele gera uma especificação completa do produto, contendo:
	1. detalhes de implantação
	2. seleções do modelo de features
	3. definições dos sensores
3. Sensor builder SPL: este componente utiliza as informações da especificação gerada para produzir o código-fonte, com base no código anotado da Software Product Line, atendendo todas as especificações definidas pelo usuário.
4. Product deployer: este componente é responsável pela implantação do produto. Atualmente, ele oferece três opções de deploy:
	1. Implantação na máquina local
	2. Implantação via SSH (Ubuntu/Debian)
	3. Implantação na AWS

![[Pasted image 20260315131309.png]]

# Cenários de Uso

## Sistema de monitoramento meteorológico
Localizado na Galícia - Espanha, o MeteoGalicia é um serviço de previsão do tempo. Ele oferece previsões e dados meteorológicos para a região, incluindo informações sobre temperatura, precipitação, velocidade do vento e condições atmosféricas.

A partir da obtenção de um conjunto de dados (dataset) do MeteoGalicia de sensores que medem: precipitação, pressão atmosférica, radiação solar, umidade, temperatura e vento. Foram apresentados os dados em nível individual de cada sensor, em seguida são definidas dimensões espaciais que agregam os sensores nos níveis de Conselho (município) e Província na Galícia.

![[Pasted image 20260315141926.png]]

A imagem acima mostra o dashboard finalizado, para facilitar a navegaçãO entre as diferentes propriedades medidas pelos sensores, as agregações e filtros da dimensão espacial são exibidos no lado esquerdo da tela, juntamente com as próprias propriedades.

Os sensores são posicionados em um mapa, e os valores de cada propriedade de medisão são mostrados em cores de acordo com a legenda.



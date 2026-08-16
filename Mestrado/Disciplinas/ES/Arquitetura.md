#engenharia-de-software 

O foco deixa de ser a organização e interfaces de classes individuais e passa a ser em unidades de maior tamanho, sejam elas pacotes, componentes, módulos, subsistemas ou serviços.


Alguns padrões arquiteturais mais comuns são:
- Camadas (duas ou três)
- Model-View-Controller (MVC)
- Microsserviços
- Orientada a mensagens
- Publish/Subscribe
- Pipes&Filters
- Cliente/Servidor
- Peer-to-peer

## Arquitetura em Camadas
A arquitetura em camadas é um dos padrões arquiteturais mais usados, desde que os primeiros sistemas de software de maior porte foram construídos nas décadas de 60 e 70. As camadas são dispostas de forma hierárquica, assim uma camada somente pode usar serviços de uma camada imediatamente inferior.

## Arquitetura em Três Camadas
Esse tipo de arquitetura é comum na construção de sistemas corporativos. As três camadas dessa arquitetura são as seguintes:
- Interface com o usuário: ela trata tando da exibição de informações, como da coleta e processamento de entradas e eventos de interfaces.
- Lógica de negócio: implementa as regras de negócio do sistema.
- Banco de dados: armazena os dados manipulados pelo sistema.

## Microsserviços
Esse modelo decompõe aplicações em pequenos serviços independentes, cada um focado em uma função específica e comunicando-se por APIs.


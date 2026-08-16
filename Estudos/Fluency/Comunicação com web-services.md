#linguagens-de-programação #backend 

# O que são web services?
Web services são sistemas ou aplicações que permitem a comunicação e a troca de dados entre diferentes sistemas e dispositivos pela internet, utilizando padrões e protocolos abertos. Eles são projetados para facilitar a interoperabilidade entre plataformas diversas e são amplamente usados para integrar aplicações e automatizar processos.

# Uma API é um web service ?
API (Application Programming Interface) trata-se de um conjunto de definições e protocolos que permite que diferentes softwares interagem entre si. Ela define os métodos e dados que os desenvolvedores podem usar para se comunicar com um serviço, biblioteca ou sistema operacional.

Web service é um tipo específico de API que permite a comunicação entre sistemas pela internet usando protocolos padrão como ==HTTP==, ==XML==, ==SOAP== ou ==REST==.

# Como funciona um web service?
![[Pasted image 20260604161900.png]]

Basicamente um dispositivo cliente (computador, celular, etc) envia uma requisição através a internet para o web service, que irá processar a requisição e enviar através da internet um retorno.

O cliente de um web service é uma aplicação ou componente de software que envia requisições a um web service para obter dados ou realizar operações.

O servidor de um web service é uma aplicação ou componente de software que recebe requisições dos clientes, processa elas e envia respostas de acordo com o requisitado.

# O que é uma arquitetura em um web service?
Em um web service, a arquitetura se refere à estrutura e às metodologias utilizadas para desenvolver, implementar e integrar o serviço na web. A arquitetura define como os componentes do web service interagem, como os dados são transmitidos e processados, e como a segurança e a escalabilidade são gerenciadas. Aqui estão as principais arquiteturas usadas em web services: Arquitetura SOAP (Simple Object Acces Protocol), Arquitetura REST (Representational State Transfer) e Arquitetura GraphQL.

- SOAP (Simple Object Acces Protocol): Um protocolo baseado em XML que permite a troca de informações estruturadas entre sistemas através de ==HTTP==, ==SMTP==, e outros protocolos.
- REST (Representational State Transfer): Um estilo arquitetural que usa ==HTTP== e é baseado em operações padrão como ==GET==, ==POST==, ==PUT== e ==DELETE==.
- GraphQL: É uma linguagem de consulta para APIs que permite aos clientes pedir exatamente os dados de que precisam.

# Como tudo isso funciona na web?
Tudo funciona através do uso de protocolos de comunicação, esses protocolos podem variar dependendo da arquitetura específica do serviço e dos requisitos do projeto. No entando, existem alguns protocolos comuns que são amplamente utilizados em diferentes tipos de web services. Aqui estão os principais: ==HTTP== (Hypertext Transfer Protocol), ==SOAP== (Simple Object Access Protocol) e ==JSON-RPC== (JSON Remote Procedure Call).
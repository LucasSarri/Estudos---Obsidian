#linguagens-de-programação #backend 

# O que é um endereço de um recurso na web (URL) ?
URL é uma abreviação de localizador uniforme de recursos, um endereço da Web que aponta para um site específico, uma página da Web ou document na Internet. Um exemplo de url é: https://nodejs.com/.

As URLs podem possuir especificidades, como quando queremos acessar um ==recurso== específico: https://nodejs.com/docs/.

Uma URL pode também enviar o usuário para uma ==seção== específica de uma página, como neste exemplo: https://nodejs.com/docs/latest/#error.

# Como é formada uma URL?
![[Pasted image 20260602182516.png]]
A primeira parte é o ==Protocolo== que define um padrão de comunicação, basicamente é um conjunto de regras e normas que define como dados são transmitidos e recebidos através de uma rede de comunicação. Existem diversos tipos de protocolos, cada um servindo a propósitos diferentes, um exemplo é o ==HTTP/HTTPS== (HyperText Transfer Protocol/Secure) que é usado para a transferência de páginas web.

O ==Domínio== representa um endereço, por baixo dos panos representa o IP. Um domínio na web é um endereço legível por humanos que identifica um local específico na internet. Ele é usado para acessar sites e recursos online de maneira fácil, em vez de utilizar endereços IP numéricos, que são difíceis de lembrar. Cada nome de domínio é único e eles representam seus endereços IP correspondentes.

A ==Porta== em uma URL tem como objetivo indicar qual é o portão técnico usado para acessar os recursos no servidor web. Usualmente ela é omitida se o servidor web utiliza a porta padrão do protocolo ==HTTP== (80 para HTTP e 443 para HTTPS) para garantir o acesso aos recursos.

O ==Caminho== em uma URL especificam a localização exata de um recurso em um servidor, geralmente especifica qual página está sendo acessada do site. Eles fazem parte da estrutura da URL e ajudam a identificar diretórios, subdiretórios, arquivos ou parâmetros específicos. A importância de utilizar caminhos se dá para uma melhor navegação, organização e SEO (Search Engine Optimization).

Os ==Parâmetros== são strings de consulta ou variáveis de URL, eles são a parte de uma URL após um ponto de interrogação. Os parâmetros contêm chaves e valores separados pelo sinal de igual (=), além disso uma URL pode ter várias variáveis, nesse caso o símblo de E comercial (&) separará cada um. Eles são utilizados para realizar pesquisas nos sites.

Um ==Fragmento== é uma âncora para outra parte do próprio recurso, uma âncora representa uma espécie de marcador dentro do recurso, dando ao navegador as instruções para mostrar o conteúco localizado naquele ponto marcado. Em um documento HTML, por exemplo, o navegador irá dar scroll para âncora em um ponto definido, em um vídeo ou áudio, o navegador irá tentar ir para o tempo que a âncora representa.
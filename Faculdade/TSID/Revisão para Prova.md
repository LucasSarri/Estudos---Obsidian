#tsid

# Introdução
Um programa distribuído possuí componentes interligados (comunicação), processamento (computação) distribuído ou paralelo.

Um sistema distribuído possuí uma maior confiabilidade, pois todas as funçõespodem ser replicadas:
* Quando um processador falha, outro pode continuar o trabalho
* Se um disco dá crash, arquivos gravados também estão gravados em outros discos, dessa forma não serão perdidos.

Várias computações podem ser realizadas em paralelo, um sistema distribuído pode realizar mais atividades na mesma quantidade de tempo.

Pode-se considerar a tolerância a falha e possibilidade de paralelismo como as propriedades fundamentais de um sistema distribuído.

# Definições
- Lamport: “Um sistema distribuído é aquele que faz você parar de ter trabalho realizado quando uma máquina na qual você nunca ouviu falar falha“
- Tanenbaum e van Renesse (1985): “Um sistema (operacional) distribuído é aquele que aparece para os usuários como um sistema (operacional) centralizado ordinário, mas que executa em múltiplas CPUs independentes. O conceito chave é a transparência, ou seja, o uso de múltiplos processadores deve ser invisível (transparente) para o usuário. Pode-se dizer que o sistema é visto como um uniprocessador virtual, e não como uma coleção de máquinas distintas.“
- “Um sistema distribuído é um conjunto de computadores autônomos interligados por uma rede com software projetado para produzir um ambiente computacional integrado para o usuário.” Coulouris et al., 2013
- “Um sistema distribuído é um conjunto de computadores independentes que se apresenta a seus usuários como sistema único e coerente.” Tanenbaum et al., 2008
- “Você sabe que tem um quando o defeito de um computador que você nunca ouviu falar lhe impede de fazer o seu trabalho.” Leslie Lamport 
- “Um sistema distribuído é um conjunto de computadores independentes que se apresenta a seus usuários como um sistema único e coerente” Tanenbaum; Van Steen, 2008

# Tipos de transparência
1. Localização: esconde onde o recurso está localizado
2. Acesso: operações idênticas para acesso local e remoto
3. Migração: esconde que um recurso pode se mover para outra localização
4. Relocação: esconde que um recurso pode ser movido para outra localização enquanto está em uso
5. Concorrência: compartilhamento de recursos sem interferência entre processos concorrentes
6. Falha: esconde a falha e recuperação de um recurso
7. Replicação: esconde de usuário ou programadores de aplicação a existência de réplicas de recursos

# Definições recentes
- Tanenbaum & van Steen: “Coleção de computadores independentes que aparecem para os usuário do sistema como um único computador.“
- Coulouris et al: “Um sistema em que componentes e hardware e software localizados em computadores em rede se comunicam e coordenam suas ações por passagem de mensagens.“
- M. Eckhouse: “Uma coleção de elementos de processamento interconectados, tanto logicamente como fisicamente, para execução cooperativa de programas de aplicação com o controle geral dos recursos centralizado.“

# Vantagens de um Sistema Distribuído
1. Relação custo/desempenho
2. Modularidade
3. Expansibilidade
4. Disponibilidade
5. Escalabilidade
6. Confiabilidade

# Complexidade
A complexidade limita o que pode ser construído, Schroeder chama os problemas causados pela complexidade de problemas de sistema:
- Interconexão: um grande número de problemas de sistemas acontece quando componentes que antes operavam independemente são interconectados.
- Interferência: dois componentes de um sistema, cada um com comportamento razoável quando observados em isolamento, podem exibir comportamento indesejável quando combinados
- Propagação de efeito: efeito cascata de falhas pode derrubar um sistema inteiro se não houver cuidados no projeto
- Efeito de escala: um sistema que funciona bem com 10 nós pode falhar se crescer para centenas de nós
- A solução simples nem sempre pode ser usada - às vezes é cara demais

# Desafios
- Heterogeneidade
- Segurança
- Escalabilidade
- Transparência
- Concorrência
- Tolerância a Falhas
- Abertura

# Características
- Heterogeneidade
- Segurança
- Escalabilidade
- Confiabilidade
- Concorrência
- Transparência
- Gerenciamento

# Middleware
“... camada de software - que é situada logicamente entre uma camada de nível mais alto, composta de usuários e aplicações, e uma camada subjacente, que consiste em sistemas operacionais e facilidades vásicas de comunicação.” Tanenbaum et al. 2008
![[Pasted image 20250630211602.png]]
O middleware é usado para mover informações entre programas ocultando diferenças de protocolos de comunicação, plataformas e dependências do sistema operacional.

# Metas
São importantes para a construção de um sistema distribuído
- Um sistema distribuído deve oferecer fácil acesso a seus recursos
- Deve ocultar razoavelmente bem o fato de que os recursos são distribuídos por uma rede
- Deve ser aberto
- Deve poder ser expandido

## Acesso a recursos
Um sistema distribuído deve oferecer fácil acesso a seus recursos, como impressora compartilhada, computadores compartilados, facilidades de armazenamento, dados, páginas web, software de edição colaborativa e videoconferência.
“A medida que a conectividade e o compartilhamento crescem, a segurança se torna cada vez mais importante“ Tanenbaum, 2008

## Transparência da distribuição
“Uma meta importante de um sistema distribuído é ocultar o fato de que seus processos e recursos estão fisicamente distribuídos por vários computadores.” Tanenbaum, 2008

“trata de oultar diferenças em representação de dados e o modo como os recursos podem ser acessados por usuários“ Tanenbaum, 2008

## Abertura
“Um sistema distribuído aberto é um sistema que oferece serviços de acordo com regras padronizadas que descrevem a sintaxe e a semântica desses serviços” Tanenbaum, 2008

## Escalabilidade
Deve poder ser expandido, pode ser medida por três dimensões diferentes:
- Escalável em relação ao seu tamanho
- Escalável em termos geográficos
- Escalável em termos administrativos

## Um sistema deve oferecer fácil acesso a seus recursos
Deve ocultar razoavelmente bem o fato de que os recursos são distribuídos por uma rede, deve ser aberto e deve poder ser expandido.

# Classificação dos sistemas distribuídos
- Sistemas de computação distribuídos
- Sistemas de informação distribuídos
- Sistemas embutivos distribuídos

## Sistemas de computação distribuídos
Utilizada para computação de alto desempenho, pode ser dividida em dois subgrupos:
- Computação de cluster: o hardware subjacente consiste em um conjunto de estações de trabalho ou PCs semelhantes, conectados por meio de uma rede local de alta velocidade. Cada nó executa o mesmo sistema operacional.
- Computação em grade: consiste em sistemas distribuídos que costumam ser montados como federação de computadores, na qual cada sistema pode cair sob um domínio administrativo diferente, e pode ser muito diferente no que tange a hardware, software e tecnologia de rede empregada.

### Sistemas de computação em grade
Tem alto grau de heterogeneidade, a colaboração é realizada através de uma organização virtual e a computação em grade tem a finalidade de prover acesso a recursos de diferentes domínios administrativos, e somente para usuários e aplicações que pertençam a uma organização virtual específica.
Camada base provê interfaces para recursos locais em um site específico, a camada de conectividade que consiste em protocolos de comunicação para suportar transações da grade que abranjam a utilização de múltiplos recursos e a camada de recursos é responsável pelo gerenciamento de um único recurso, ela utiliza funções fornecidas pela camada de conectividade e chama diretamente as interfaces disponibilizadas pela camada-base. A camada coletiva trata de manipular o acesso a múltiplos recursos e normalmente consiste em serviços para descoberta de recursos, alocação e escalonamento de tarefas para múltiplos recursos, replicação de dados e assim por diante e por fim a camada de aplicação consiste em aplicações que funcionam dentro de uma organização virtual e que fazem uso do ambiente de computação em grade.

### Sistemas de informação distribuídos
“Muitas das soluções e middleware existentes são resultado do trabalho com uma infraestrutura na qual era mais fácil integrar aplicações a um sistema de informações de âmbito empresarial” Tanenbaum, 2008

#### Sistemas de processamento de transações
São baseados em aplicações que realizam operações sob a forma de transações, isso requer primitivas especiais que devem ser fornecidas pelo sistema distribuído subjacente ou pelo sistema de linguagem em tempo de execução.

#### Integração de aplicações empresariais
“Quanto mais aplicações se desvinculam dos bancos de dados sobre os quais eram construídas, mais evidente ficava que eram necessárias facilidades para integrar aplicações independentemente de seus bancos de dados.” Tanenbaum, 2008
Propostas de middleware:
- RPC (Remote Procedure Call)
- RMI (Remote Method Invocations)

### Sistemas distribuídos pervasivos
São sistemas distribuídos tal qual foi visto até aqui, porém, a instabilidade é o comportamento esperado dos equipamentos do sistema. Eles costumam ser pequenos, móveis, e geralmente tem uma conexão sem fio. 
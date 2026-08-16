https://dl.acm.org/doi/10.1145/3696630.3727241

# Introdução
Uma abordagem pedagógica que apoia essa perspetiva é a aprendizagem baseada em projetos (PBL, do inglês _project-based learning_), na qual os estudantes se envolvem em projetos reais que exigem a aplicação de conhecimentos teóricos a tarefas práticas [6]. No ensino de ES, a PBL é frequentemente aplicada em "projetos estudantis de desenvolvimento de software", nos quais se utilizam muitas vezes processos ágeis de desenvolvimento, como o Scrum [49], para familiarizar os estudantes com requisitos mutáveis de clientes provenientes de diversas partes interessadas, o trabalho em sprints e revisões frequentes do produto[42].

Os estudantes têm frequentemente dificuldade em aprender novas tecnologias e, geralmente, possuem pouca ou nenhuma experiência prévia no trabalho com sistemas de software mais extensos e no desenvolvimento de software em equipas maiores. Além disso, a comunicação e a coordenação dentro da equipa podem ser desafiantes, e uma distribuição desigual do trabalho pode gerar frustração. A baixa motivação é um fator crítico para o fracasso de projetos de desenvolvimento de software [63], pois conduz a um fraco envolvimento com as tarefas, ao atraso de marcos e a uma colaboração subótima. Assim, é benéfico para todas as partes envolvidas nesses projetos investigar formas de motivar os estudantes.

Uma abordagem para aumentar a motivação dos estudantes é a gamificação, ou seja, a aplicação de elementos de design de jogos em contextos não lúdicos [12]. Assim, neste artigo, enfrentamos os desafios enunciados e apresentamos o conceito e a ferramenta DinoDev para a implementação de gamificação em projetos estudantis de desenvolvimento de software. A gamificação tem sido bem-sucedida em vários domínios, incluindo a educação e a ES [1, 14, 46]. A combinação da gamificação com a PBL, também designada por "aprendizagem baseada em projetos gamificada" (GPBL, de _gamified project-based learning_), é uma abordagem promissora para melhorar os resultados de aprendizagem dos estudantes [20].

RQ1: “A implementação de gamificação aumenta a motivação dos estudantes em projetos estudantis de desenvolvimento?”  
RQ2: “A implementação de gamificação aumenta a produtividade da equipa em projetos estudantis de desenvolvimento?”  
Ao responder a estas questões de investigação, pretendemos impulsionar a investigação futura na área da motivação dos estudantes e da gamificação no ensino de ES, e capacitar os docentes com uma abordagem de gamificação para aumentar a motivação dos estudantes e a produtividade da equipa nos seus projetos estudantis de desenvolvimento de software. Um vídeo de demonstração do protótipo DinoDev implementado está disponível no YouTube1.

Em resumo, as nossas contribuições são: (1) um conjunto de requisitos elicitados para a gamificação em cursos de PBL, (2) uma análise das preocupações, benefícios percecionados e restrições dos orientadores, (3) um conceito de gamificação para cursos de PBL que incorpora gestão ágil de projetos gamificada, gamificação orientada para a equipa e gamificação orientada para o estudante, e (4) um protótipo que implementa estes conceitos, integra de forma harmoniosa os eventos Scrum e pode ser utilizado com uma variedade de sistemas tradicionais de acompanhamento de tarefas.

# Student Software Development Projects
Os projetos estudantis de desenvolvimento de software são uma forma de PBL e são parte integrante da formação em ES para engenheiros de software devido ao seu foco prático [42]. Estes projetos têm como objetivo facilitar a capacidade dos estudantes para desenvolverem, em conjunto como equipa, sistemas de software maiores e mais complexos, com base nos requisitos dos "clientes" (ou seja, os orientadores e examinadores). Isto promove tanto as competências práticas como as competências interpessoais dos estudantes, que aprendem a organizar-se em equipa, de forma semelhante ao desenvolvimento de software real na indústria e em código aberto [39].

O projeto de licenciatura corresponde a 15 pontos ECTS (450 horas por estudante), e o projeto de mestrado a 12 pontos ECTS (360 horas por estudante). Por conseguinte, espera-se que os estudantes já tenham concluído disciplinas de programação e de processos de ES. Nestes projetos, seguimos um método de desenvolvimento ágil de software (tipicamente Scrum) com sprints de duas ou três semanas. Um estudante assume explicitamente o papel de Product Owner e, na maioria dos casos, outro estudante é o Scrum Master da equipa e gere a equipa de desenvolvimento e a comunicação com o cliente. Assim, os estudantes seguem os eventos Scrum típicos, como as Sprint Plannings, as Sprint Reviews e as Sprint Retrospectives.

# Related Work
A investigação na área da gamificação sugere que a sua eficácia depende do contexto em que é implementada e dos utilizadores do sistema gamificado [17]. Estudos anteriores revelam resultados promissores tanto em ES como na educação [1, 14, 46]. No entanto, muitas vezes é utilizada apenas uma pequena seleção de elementos de jogo simples nesses estudos [16, 29, 40]. Por conseguinte, identificamos a necessidade de um conceito de gamificação mais abrangente, que considere uma gama mais ampla de elementos e mecânicas de jogo.

o nosso trabalho visa gamificar os processos ágeis de ES. Existem várias abordagens para um processo Scrum gamificado: (1) O ScrumHero [44] é um conceito para a utilização da gamificação no planeamento e gestão de projetos Scrum. Inclui vários mecanismos de recompensa e pontuação, e substitui a terminologia Scrum por designações lúdicas, como "lista de desejos" em vez de Product Backlog. (2) De forma semelhante, Hermanto et al. [18] conceberam um protótipo de uma ferramenta Scrum que utiliza elementos de jogo simples, incluindo um perfil de utilizador e uma tabela de classificação. Para ambas as abordagens, não conseguimos encontrar uma validação empírica. (3) Em contrapartida, Marques et al. [31, 32] implementaram e avaliaram uma aplicação para o Atlassian JIRA que utiliza uma variedade de elementos de jogo com o objetivo de aumentar a motivação da equipa para aplicar as práticas Scrum.

O objetivo de ensinar a metodologia Scrum com GPBL também foi investigado na literatura. Sisomboon et al. [52] procuraram melhorar o envolvimento e a motivação em projetos de ES baseados em Scrum, incorporando elementos de jogo simples, como pontos, distintivos, tabelas de classificação e desafios, mas a sua abordagem não envolve o desenvolvimento de uma plataforma gamificada nem a integração com sistemas externos. Os tijolos Lego [8, 19], os quadros Miro [13] ou o videojogo Minecraft [50] permitem substituir os aspetos técnicos do desenvolvimento de software por uma atividade mais lúdica e focam-se inteiramente no ensino do Scrum.

Além das abordagens de gamificação, as ferramentas de gestão de projetos de ES para o contexto educativo são escassas. Embora a utilização de ferramentas padrão da indústria em projetos estudantis de desenvolvimento possa estar mais próxima de um ambiente real, ferramentas especializadas podem permitir que os orientadores avaliem a aprendizagem dos estudantes e identifiquem problemas no projeto, tais como padrões de trabalho pouco saudáveis ou estudantes isolados na equipa. Isto é conseguido pela ferramenta de gestão de projetos ScrumBoard [37]. Esta foi especificamente concebida para o ensino de ES e é semelhante às ferramentas padrão da indústria. Vemos potencial em adicionar funcionalidades semelhantes de avaliação de estudantes no DinoDev em implementações futuras.

# 5 - Gamification Concept
O conceito de gamificação proposto combina funcionalidades de **gerenciamento de projetos e tarefas** voltadas para projetos de desenvolvimento de software realizados por estudantes com elementos de gamificação definidos a partir dos requisitos e da análise de usuários apresentados na Seção 4.

O conceito é dividido em quatro partes:

1. **Funcionalidades de gerenciamento de projetos** que incentivam o uso da ferramenta desenvolvida, fornecendo recursos para apoiar o processo Scrum.
2. **Elementos de gamificação orientados à equipe**, com o objetivo de aumentar a motivação para o trabalho colaborativo, fortalecer o espírito de equipe e incentivar o alcance dos objetivos do projeto.
3. **Elementos de gamificação orientados ao estudante**, destinados a aumentar a motivação individual dos alunos para que cumpram suas responsabilidades e entreguem suas atividades com dedicação e confiabilidade.
4. **Eventos Scrum**, projetados para consumir o menor tempo possível, aumentar a produtividade e a eficácia das reuniões e incentivar a participação ativa de cada estudante.

Devido ao tema de dinossauros adotado pela plataforma e à visão do projeto **IT-REX** [56], que busca criar um ambiente de aprendizagem gamificado para estudantes de Computação nos primeiros semestres, o tema dos dinossauros também foi adotado no DinoDev.

Assim, a ideia central do DinoDev é que os estudantes de um projeto **choquem e criem um dinossauro como mascote de cada sprint** (Figura 3).

Cada tarefa concluída por um estudante contribui para o crescimento do dinossauro.

- Se a equipe concluir todas as tarefas planejadas para a sprint, o dinossauro cresce completamente.
- Na sprint seguinte, a equipe pode iniciar a criação de um novo dinossauro.

Dessa forma, ao longo do tempo é criado um **parque de dinossauros**, contendo diferentes espécies, onde cada dinossauro representa uma sprint concluída com sucesso.

Por outro lado, se a equipe falhar em uma sprint, o dinossauro correspondente deve deixar o parque, representando visualmente as consequências de não concluir todas as tarefas planejadas.

## 5.1 - Project Management Concept
O objetivo é fornecer aos estudantes uma ferramenta que seja útil para o processo de desenvolvimento de software mesmo sem os elementos de gamificação.

Como já existem diversos **Sistemas de Gerenciamento de Issues (Issue Management Systems - IMS)**, a proposta concentra-se em funcionalidades que normalmente não são oferecidas por ferramentas tradicionais, como GitHub Projects ou Atlassian JIRA.

Uma funcionalidade comum desses sistemas é o **Quadro Kanban**, que exibe as tarefas em colunas correspondentes aos seus estados de trabalho. O DinoDev também oferece um quadro desse tipo, porém com extensões adicionais:

- Avisos quando o usuário tenta realizar mudanças incomuns de estado, como mover uma tarefa concluída de volta para o backlog;
- Exibição de uma janela de confirmação ao encerrar uma tarefa, lembrando o usuário da **Definition of Done (DoD)** configurada para o projeto.

Na página principal do DinoDev são exibidos apenas os eventos considerados mais relevantes, incluindo:

- Criação de tarefas;
- Conclusão de tarefas;
- Abertura de Pull Requests;
- Mesclagem (merge) de Pull Requests.

Outras funcionalidades de gerenciamento de projetos incluem:

- Visualização de estatísticas, como a velocidade da sprint;
- Criação e comentários em tarefas;
- Suporte à execução dos eventos Scrum (descrito na Seção 5.4).

Para evitar a necessidade de desenvolver um novo sistema completo de gerenciamento de tarefas do zero, o DinoDev foi projetado para integrar informações provenientes de sistemas já existentes.

Dessa forma, a ferramenta depende de:

- Dados de tarefas provenientes de um IMS já existente;
- Dados de Pull Requests provenientes de um Sistema de Repositório de Código (Code Repository System - CRS), como o GitHub.

Assim, o DinoDev foi concebido para funcionar em conjunto com um IMS e um CRS já estabelecidos, combinando:

- As vantagens de softwares amplamente utilizados no mercado;
- As funcionalidades personalizadas e gamificadas da ferramenta.

Embora isso ocasionalmente exija que os usuários alternem entre diferentes sistemas, essa abordagem evita redundância e reduz significativamente o esforço de implementação.

A comunicação com os sistemas externos é realizada por meio de **adaptadores (adapters)**.

Esses adaptadores são responsáveis por:

- Converter os dados dos sistemas externos para o modelo interno do DinoDev;
- Converter informações do DinoDev para o formato esperado pelos sistemas externos.

Essa arquitetura permite que a ferramenta seja facilmente expandida para trabalhar com outros sistemas que disponibilizem APIs, aumentando sua flexibilidade e reutilização.

## 5.2 - Team-Oriented Gamification
O conceito de gamificação orientado à equipe tem como objetivo motivar o grupo como um todo a alcançar a meta da sprint, trabalhar de forma colaborativa, produtiva e apoiar uns aos outros. Para isso, foram consideradas as seguintes áreas:

### 5.2.1 - Parque dos Dinossauros
O Parque dos Dinossauros foi concebido para criar incentivos que estimulem o alcance das metas da sprint e o aumento da velocidade da equipe.

Em vez de utilizar um zoológico com animais virtuais, optou-se por um parque de dinossauros, alinhado à plataforma educacional temática de dinossauros IT-REX, voltada para estudantes de Ciência da Computação [56].

No início de cada sprint, a equipe pode votar na espécie de dinossauro que deseja chocar como mascote da sprint. Inicialmente, apenas algumas espécies estão disponíveis, mas novas espécies podem ser desbloqueadas à medida que a equipe aumenta sua velocidade de sprint. Além disso, os membros podem escolher um nome para o dinossauro.

### 5.2.2 - Interações sociais
O sistema utiliza diversos elementos interativos que incentivam as interações sociais entre os membros da equipe.

Primeiramente, é possível publicar mensagens na visão geral de atividades do projeto, visíveis para todos os integrantes da equipe (Figura 4). Os estudantes também podem responder a essas mensagens globais.

O mesmo ocorre com as mensagens relacionadas às issues (tarefas). Essas mensagens são sincronizadas com o Sistema de Gerenciamento de Issues (IMS) subjacente, garantindo que todos os membros da equipe estejam informados sobre as discussões.




# 1 - Introduction
O ensino de **Engenharia de Software (ES)** para estudantes de graduação apresenta um conflito inerente. Enquanto a ES é voltada para sistemas complexos e de grande escala, que exigem estabilidade, interoperabilidade e confiabilidade, entre outras qualidades, o ensino de ES é inevitavelmente limitado a sistemas pequenos, de curta duração e relativamente simples, nos quais a integração efetiva de uma ampla variedade de competências de engenharia de software não é realmente essencial.

A **Aprendizagem Baseada em Problemas (Problem-Based Learning – PBL)** é uma abordagem educacional emergente que possibilita a **Aprendizagem Integrativa (Integrative Learning – IL)** e a prática em diversos paradigmas, incluindo a Engenharia de Software. No PBL, o trabalho dos estudantes é organizado em torno da resolução de um problema complexo, possivelmente mal estruturado, que envolve conteúdos autênticos relacionados à disciplina.

Na abordagem tradicional de aprendizagem baseada em projetos, a responsabilidade pela integração dos conhecimentos recai inteiramente sobre os estudantes. Esses cursos geralmente não fornecem uma base metodológica e sistemática para o desenvolvimento de habilidades integrativas em Engenharia de Software.

A ampla experiência dos autores no ensino de ES demonstra que a **Aprendizagem Integrativa não surge espontaneamente durante o trabalho em projetos**. As habilidades de integração precisam ser ensinadas, praticadas e vivenciadas dentro de uma estrutura pedagógica planejada.

# A Framework for Practicing Integration Skills in SE Education
Nesta seção, apresentamos um framework para a prática da **Aprendizagem Integrativa (Integrative Learning - IL)** no ensino superior de Engenharia de Software (ES). O framework foi concebido para ser utilizado por estudantes que já tenham aprendido diferentes tópicos da área de ES e que ainda não tenham iniciado um projeto final independente (como um trabalho de conclusão ou projeto de graduação).

# Application of the SE-IL-Framework in Anonymized University
Ele faz parte de um currículo que inclui disciplinas básicas e avançadas de Ciência da Computação e Engenharia de Software, abrangendo programação, bancos de dados, modelagem de software, qualidade de software, comunicação, redes e verificação de software. O curso é ministrado antes da disciplina de projeto final de graduação. O material do curso está disponível em [1].

## Contexto e Problema
O problema desafiador escolhido para o curso é o desenvolvimento de uma aplicação robusta para um sistema de comércio eletrônico.

O problema é definido por meio de especificações de requisitos elaboradas pela equipe docente, juntamente com uma metodologia para gerenciamento do projeto, desenvolvimento e colaboração entre os desenvolvedores.

Os requisitos foram cuidadosamente elaborados para promover a integração das habilidades-alvo:

- Abstração;
- Coordenação eficiente entre equipes;
- Domínio abrangente dos conhecimentos de Engenharia de Software.
## Princípios de Projeto dos Requisitos

#### (a) Especificação independente de plataforma e tecnologia

> “Um sistema de comércio é uma infraestrutura de negociação que dá suporte a compradores e vendedores, incluindo lojas identificadas e produtos identificados. Compradores podem entrar e sair livremente, abrir lojas e atuar como vendedores.”

Essa especificação pode representar tanto um mercado físico quanto um mercado virtual.

A independência de plataforma obriga os estudantes a focarem na essência dos requisitos, reduzindo a dependência de tecnologias específicas.

#### (b) Distinção entre SLO, SLI e SLA

O curso enfatiza a separação entre:

- **SLO (Service Level Objectives)**: objetivos abstratos do sistema;
- **SLI (Service Level Indicators)**: indicadores específicos da plataforma utilizados para medir os objetivos;
- **SLA (Service Level Agreements)**: acordos de desempenho definidos com base nos indicadores.

#### (c) Utilização de diversos elementos computacionais

O sistema deve incorporar uma ampla variedade de componentes computacionais, tanto internamente quanto em sua interação com o ambiente externo.

#### (d) Uso de tecnologias modernas de Engenharia de Software

Incluindo aspectos como:

- Privacidade;
- Tecnologias de integração e troca de dados;
- Experiência do usuário;
- Escalabilidade;
- Operação contínua;
- Recuperação de falhas;
- Armazenamento de dados;
- Rastreabilidade.

#### (e) Alta qualidade de software

Os requisitos do projeto também foram desenhados para exigir diversos atributos de qualidade:

##### Manutenibilidade

Exige uma arquitetura baseada em componentes e a separação entre a lógica de negócio e os serviços sujeitos a mudanças frequentes.

##### Confiabilidade

Exige um mecanismo de testes abrangente e bem arquitetado.

##### Robustez e Disponibilidade

Exigem um projeto indireto, capaz de lidar com falhas em serviços externos e interrupções na comunicação.

##### Flexibilidade e Rastreabilidade

Exigem dependências cuidadosamente estruturadas entre requisitos, código-fonte e testes.

##### Abstração Conceitual

Incluindo conceitos como:

- Sensibilidade a estados (_state sensitivity_);
- Abstração funcional.

## Ciclos de Trabalho (Rounds)

O desenvolvimento do projeto é dividido em **quatro ciclos (rounds)**.

As tarefas de cada ciclo são escolhidas para desafiar os participantes a integrar as diferentes práticas de Engenharia de Software que estão sendo aplicadas.

As atividades de cada ciclo são detalhadas em um documento de especificação próprio (disponível no apêndice online [1]).
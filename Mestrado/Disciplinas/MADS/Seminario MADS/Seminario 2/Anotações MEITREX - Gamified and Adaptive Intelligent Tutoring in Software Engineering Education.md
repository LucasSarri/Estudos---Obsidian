
https://dl.acm.org/doi/10.1145/3639478.3639804

# 1 - Problema
Na educação em ES, há uma ênfase especial no desenvolvimento das habilidades práticas dos estudantes [10], o que exige uma quantidade significativa de feedback por parte dos docentes. No entanto, os sistemas tradicionais de gestão da aprendizagem (_Learning Management Systems_ – LMSs) não foram projetados para atender às necessidades dessa educação prática orientada à engenharia de software, fazendo com que os professores dependam de ferramentas externas adicionais da área de ES.

# 2 - Trabalhos relacionados
O **ArTEMiS**, de Krusche e Seitz [22], é uma ferramenta de avaliação automática para cursos interativos de programação, que também pode ser utilizada como um sistema de gestão da aprendizagem (_Learning Management System_ – LMS) e continua sendo aprimorada continuamente. No entanto, o feedback individual fornecido pela ferramenta concentra-se na avaliação do código-fonte produzido pelos estudantes, sem considerar análises mais amplas sobre o processo de aprendizagem dos alunos em ES, tampouco aspectos relacionados à aprendizagem adaptativa e à motivação estudantil.

Ferramentas comerciais, como o **MATHia**, da Carnegie Learning Inc. [9], analisam os estudantes com base em suas respostas, fornecem feedback apropriado e oferecem recursos de aprendizagem adaptativa. Entretanto, essas ferramentas não são direcionadas à educação em Engenharia de Software e estão limitadas ao contexto do ensino básico e médio.

As revisões sistemáticas realizadas por Crow et al. [11] e Nesbit et al. [33] sobre **Sistemas Tutores Inteligentes** (_Intelligent Tutoring Systems_ – ITSs) aplicados à Ciência da Computação, Engenharia de Software e ensino de programação mostram que alguns pesquisadores desenvolveram ITSs que incorporam elementos de jogos e permitem que estudantes programem robôs ou artefatos semelhantes. Outra tendência observada em alguns ITSs é o monitoramento e a modelagem do estado emocional dos estudantes, com o objetivo de fornecer suporte pedagógico e estratégico [33].

# 3 - PROPOSED APPROACH
Para enfrentar o problema identificado, propomos o desenvolvimento do **MEITREX** (_Modular Embedded Intelligent Tutoring and Remote Education eXperience_), uma abordagem inovadora destinada a tornar a educação em Engenharia de Software (ES) mais envolvente e motivadora, fornecendo a cada estudante feedback individualizado e elementos de aprendizagem adaptados ao seu progresso. O MEITREX é um **Sistema Tutor Inteligente** (_Intelligent Tutoring System_ – ITS) desenvolvido especificamente para o ensino superior em Engenharia de Software.

O MEITREX combina conceitos das áreas de **learning analytics**, feedback e aprendizagem interativa, como gamificação, em um único sistema, adaptando-os às necessidades da educação em Engenharia de Software. Uma visão geral dos componentes do MEITREX é apresentada na Figura 1.

Um dos principais aspectos do sistema proposto é sua capacidade de adaptação para atender ao progresso de aprendizagem e às preferências individuais de estudantes com diferentes perfis, oferecendo suporte da forma mais eficaz possível [40, 42]. Para isso, o sistema coleta e analisa informações dos estudantes (_learning analytics_), incluindo suas respostas e comportamentos de aprendizagem, estilos de aprendizagem preferidos, ritmo de estudo e conhecimentos prévios.

Com base nos dados coletados, o MEITREX adapta seu feedback para cada estudante individualmente, incluindo estratégias de feedback [32], recomendações e elementos de aprendizagem interativa, como gamificação e **repetição espaçada** (_spaced repetition_) [39]. O foco no progresso individual dos estudantes permite que o MEITREX crie uma experiência personalizada de educação em Engenharia de Software.

O sistema será utilizado para testar a hipótese de que uma abordagem de tutoria inteligente adaptativa e gamificada exerce impacto positivo na motivação dos estudantes e em sua experiência de aprendizagem em Engenharia de Software. Nesse contexto, a **Taxonomia de Bloom** [21] pode desempenhar um papel fundamental na integração dos diferentes conceitos em um único sistema, permitindo que os estudantes sejam categorizados de acordo com suas competências.

# 4 - EXPECTED CONTRIBUTIONS
Pretendemos realizar **três contribuições principais** para apoiar e motivar estudantes na educação em Engenharia de Software (ES):

1. **A primeira contribuição** consistirá na exploração da diversidade dos estudantes no domínio da Engenharia de Software e dos problemas relacionados presentes nos sistemas tradicionais de gestão da aprendizagem (_Learning Management Systems_ – LMSs).
2. **A segunda contribuição** terá como foco a análise da aprendizagem dos estudantes (_learning analytics_), utilizando um modelo de _machine learning_ desenvolvido especificamente para a educação em Engenharia de Software, com o objetivo de analisar o desempenho dos alunos.
3. **A terceira contribuição** concentrar-se-á na adaptação de componentes de aprendizagem interativa, como elementos de gamificação, com base nas preferências individuais dos estudantes e nos dados de desempenho obtidos nas contribuições (1) e (2).

Os componentes de feedback do **MEITREX** (apresentados na Figura 1) serão desenvolvidos paralelamente por outros estudantes de doutorado envolvidos no projeto.


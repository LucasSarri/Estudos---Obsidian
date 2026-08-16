
# Título
"Dívida técnica não é apenas técnica: um estudo de caso industrial em desenvolvimento ágil de software em larga escala".

# Resumo
"Organizações de software de todos os tamanhos são afetadas pelo fenômeno da ==dívida técnica==. As grandes organizações, no entanto, estão mais propensas aos seus aspectos ==não técnicos== devido ao ==grande número de equipas de diferentes dimensões==, à ==heterogeneidade de conhecimento especializado== e à ==necessidade de gestão e comunicação contínuas==. Isto é ainda mais acentuado em contextos de desenvolvimento ágil de software em larga escala, devido ao foco nas interações pessoais e na colaboração em equipa, o que consequentemente representa ==um desafio pelo aumento significativo dos caminhos de comunicação==. O objetivo deste estudo é investigar ==os aspetos não técnicos da dívida técnica no contexto do desenvolvimento ágil de software em larga escala==. Para atingir este objetivo, foi conduzido um estudo de caso envolvendo ==quatro empresas internacionais==. Durante o estudo, foram entrevistados ==24 especialistas e as suas respostas foram analisadas através de uma abordagem de investigação qualitativa==. A análise resultou em cinco aspetos não técnicos, nomeadamente: dinâmicas sociais, processo, pessoas, documentação e aspetos de requisitos, e os seus indicadores, que são específicos num contexto ágil de larga escala. Os resultados do estudo sugerem que a ==falta de comunicação, colaboração e cooperação são os principais contribuintes para os aspetos de dívida identificados, para a acumulação de dívida técnica através destes aspetos não técnicos==, e que muitas das causas decorrem de uma cultura de não desenvolvimento de regras, protocolos ou diretrizes.".

- **Dúvidas**: quatro empresas internacionais são suficientes ? 24 especialistas são suficientes?

# Introdução
Para manter a competitividade, as organizações utilizam uma ampla variedade de ferramentas e métodos para otimizar seus fluxos de trabalho operacionais. Apesar desses esforços ineficiências ou atritos nos processos organizacionais podem precipitar tanto desafios óbvios, como incapacidade de atender plenamente às demandas dos clientes, quanto problemas mais insidiosos, coletivamente denominados de deficiências de qualidade interna ou Dívida Técnica (TD)(Ramač et al., 2022). Sistemas sobrecarregados com TD acumulada podem entregar valor imediato aos clientes, no entando esse valor é frequentemente comprometido durante as fases subsequentes de desenvolvimento, incorrendo em custos significativos a longo prazo.

- **Dúvidas**: Qual é a definição de Dívida Técnica (Technical Debt TD) ?

O fenômeno da TD tem recebido atenção acadêmica substancial nos últimos anos (Berenguer et al., 2021; Behutiye et al., 2017; Rios et al., 2018), revelando sua presença ==uíbqua== no setor de TI. Tanto empresas pequenas quanto as grandes estão suscetíveis ao acúmulo de TD. Artefatos de software como código, testes e arquitetura servem como portadores primários de TD, no entanto pesquisas recentes destacam que artefatos não técnicos como as relações entre as pessoas e suas organizações desempenham um papel fundamental na criação de condições que aceleram a criação de TD.

Seguindo estas percepções o estudo utiliza o termo Dívida Não Técnica (NTD) para englobar as dinâmicas sociais e organizações que criam condições para a criação de TDs ou amplificação das já existentes. Ao longo do estudo é examinado como os aspectos não técnicos interagem sistematicamente e contribuem para a geração de TDs em contextos Ágies de Larga Escala (LSA). Para compreender a acumulação de TDs em contextos de larga escala é necessário reccorer à teoria da coordenação (Malone e Crowston, 1994), a quadros de aprendizagem organizacional (Argote e Argote, 2013) e ao pensamento de sistemas sociotécnicos (Mintzberg, 1980; Herbsleb, 2007), e não apenas a quadros de engenharia de software isoladamente. Os padrões recursivos entre dinâmicas sociais e compromissos técnicos, ou entre a volatilidade dos requisitos e as ineficiências do processo.

# Trabalho Relacionado
O desenvolvimento ágil de software transformou a forma como equipes desenvolvem e entregam software, enfatizando a flexibilidade, a colaboração e o progresso iterativo. No entando metodologias ágeis tradicionais foram concebidas para equipes pequenas e localizadas no mesmo espaço físico. À medida que as organizações enfrentam projetos cada vez mais complexos e de grande escala, com múltiplas equipes, dependências e partes interessadas, surgiu a necessidade de frameworks ágeis de larga escala. O desenvolvimento Ágil de Larga Escala (LSA) adapta os princípios ágeis para coordenar esforços entre numerosas equipes, assegurando o alinhamento com os objetivos organizacionais, mantendo a velocidade e adaptabilidade.

## Aspectos não técnicos contribuindo para TD
Na literatura são identificados vários aspectos não técnicos que contribuem para a acumulação de TDs em contextos de desenvolvimento de software, esses aspectos estão relacionados a condições organizacionais, sociais e relacionadas com o processo que criam pressões que levam a compromissos técnicos.

### Dívida Social
A dívida social está associada ao impacto do ambiente nos programadores, pode ser causada por omissões, mau comportamento e outros. Estes desafios se acumulam como dívida social, conduzindo a geração e acumulo de TDs, que em última análise afeta a qualidade do software.

### Dívida de processo
As dívidas de processo estão relacionadas a atividades de desenvolvimento que alcançam benefícios no curto prazo, mas que a longo prazo representam dificuldadesno desenvolvimento. Ocorre entre outros motivos à presença de muitas reuniões que ocorrem para a coordenação das equipes, perturbando a eficiência dos programadores. 

### Dívida de pessoas
A dívida de pessoas está associada às relações interpessoais na organização que podem levar ao abrandamento ou atraso das atividades de desenvolvimento. As dívidas de pessoas em ambientes LSA envolvem a coordenação e o alinhamento dos esforços de múltiplas quipes, products owners, e outras partes interessadas distribuídas em diferentes localizações.

### Dívida de documentação
A dívida de documentação está associada à documentação em falta, inadequada ou incompleta utilizada no projeto. Uma vez que a documentação é inadequada ou incompleta conduz a conhecimento insuficiente ou em falta entre os programadores, levando a problema de desenvolvimento.

### Dívida de requisitos
No contexto de desenvolvimento de software, a dívida de requisitos é definida como a discrepância entre o conjunto ideal de requisitos e aqueles que são especificados e implementados em um projeto. A dívida de reqisitos surge quando requisitos incompletos, ambíguos ou mal definidos são transportados para frente, frequentemente devido a restrições de tempo, colaboração inadequada das partes interessadas ou necessidades evolutivas do projeto. As consequências da dívida de requisitos não gerida podem ser profunda, afetando não só os resultados técnicos, mas também prazos e custos de projeto.

# Método de pesquisa
Este estudo utiliza uma metodologia de investigação de estudo de caso, seguindo as diretrizes estabelecidas para a realização de estudos de caso em engenharia de software, conforme descrito por Runeson et al. (2012).
Especificamente, o estudo envolve quatro grandes organizações de software, cada uma representando uma unidade de análise separada. O objetivo partilhado é explorar e compreender a Dívida Não Técnica (NTD), enquanto o contexto comum em que o estudo se insere é o desenvolvimento Ágil de Larga Escala (LSA).

Para abordar o objetivo de investigação declarado, que é investigar a NTD no contexto do desenvolvimento de software LSA, são respondidas as seguintes Questões de Investigação (RQs):  
• Quais são os aspetos não técnicos que contribuem para a dívida técnica no desenvolvimento de software LSA?  
• Quais são os indicadores dos aspetos da dívida não técnica no desenvolvimento de software LSA?

## Coleta de dados
A recolha de dados baseou-se principalmente em entrevistas semiestruturadas com profissionais, o que significa que os investigadores definiram os tópicos de alto nível e permitiram que os participantes da entrevista, ou entrevistados, partilhassem as suas opiniões sobre esses tópicos. O papel dos investigadores no processo de entrevista foi garantir que os entrevistados se mantivessem focados no tópico em questão e manter a sua motivação com perguntas ou comentários adicionais. Os entrevistados selecionados tinham diferentes funções nas suas empresas, e essas funções situavam-se tanto no lado de gestão como no lado técnico do processo de LSA.

Os tópicos da entrevista, que orientaram o processo de entrevista, com detalhes para perguntas e comentários adicionais, são os seguintes:

1. Introdução: formação do entrevistado, função, experiência e a sua visão sobre a forma de trabalhar ágil
2. Produto: qual é o produto, principais partes interessadas, principais utilizadores finais
3. Equipas Ágeis e de Desenvolvimento: Scrum, requisitos, métricas, qualidade, segurança
4. Comunicação, Colaboração e Partilha de Conhecimento: eficácia, obstáculos, exemplos
5. Perceção de segurança: envolvimento na tomada de decisão, sentimento de pertença, honestidade, exemplos
6. Dívida Não Técnica: partes obsoletas do trabalho, políticas ineficientes, melhorias, clareza das regras, confiança, normas culturais

## Análise dos Dados
Os dados coletados foram analisados utilizando a Análise por Template (TA), onde foram analisadas as transcrições das entrevistas e as anotações das observações. 
A metodologia utiliza principalmente a codificação qualitativa e o template como ferramentas de análise

# Resultados
Esta seção apresenta inicialmente as empresas participantes do estudo de caso e os entrevistados e, em seguida, apresenta cinco aspectos da Dívida Técnica Não Técnica (NTD) identificados no desenvolvimento de LSA.

## Empresas participantes e entrevistados
Quatro grandes empresas internacionais que utilizam práticas ágeis para o desenvolvimento de software participaram deste estudo de caso. Ao todo foram entrevistados 24 profissionais das empresas participantes, desses 54% ocupavam casos gerenciais e 46% ocupavam funções ténicas, incluindo desenvolvedores, testadores e analistas.

## Aspectos da dinâmica social
Nos projetos de LSA, os aspectos da dinâmica social surgem como um fator fundamental que contribui para a Dívida Técnica (TD), influenciando profundamente a produtividade das equipes. Diferentemente dos aspectos técnicos, que degradam principalmente a qualidade do software, os aspectos da dinâmica social surgem da complexidade de gerenciar as interações humanas dentro e entre equipes em ambientes ágeis.

### Sensação de alienação
Nos processos de desenvolvimento de LSA, esse indicador frequentemente surge de equipes voltadas para si mesmas, negligenciando as interações entre equipes. Esse padrão de comportamento apareceu em 18 das 24 entrevistas com participantes, abrangendo os quatro casos.

### Comunicação
A comunicação é um elemento fundamental das práticas ágeis; entretanto, em contextos de LSA, ela se torna uma fonte de problemas devido à dependência de plataformas digitais, às diferenças de fuso horário e às diferenças culturais. Os métodos ágeis tradicionais priorizam a interação presencial, o que frequentemente é impraticável em ambientes distribuídos, levando à diminuição da compreensão mútua e ao desalinhamento em relação aos objetivos do projeto.

## Aspectos relacionados aos processos
Os aspectos relacionados aos processos que contribuem para a TD surgem de ineficiências no fluxo de trabalho e na adesão às metodologias ágeis, que podem se tornar desalinhadas ou desatualizadas ao longo do tempo. Diferentemente da TD, que afeta diretamente a base de código, os aspectos relacionados aos processos decorrem de práticas abaixo do ideal ou mal implementadas, que reduzem a produtividade e a eficiência da equipe.

### Cerimônias ágeis excessivas
As cerimônias ágeis excessivas foram mencionadas em 21 das 24 entrevistas, abrangendo todos os casos, tornando-se um dos indicadores de processo mais frequentemente citados. O impacto foi mais grave em C2 e C3, onde a coordenação entre diferentes fusos horários exigia inúmeras reuniões de sincronização.

As cerimônias excessivas em projetos de LSA, impulsionadas pela coordenação entre fusos horários e pelas dependências entre equipes, frequentemente sobrecarregam os membros das equipes, prejudicando a produtividade. Aspectos relacionados à fadiga causada por reuniões foram observados em 21 das 24 entrevistas, em todos os casos.

### Retrospectivas ineficazes
As reuniões retrospectivas são fundamentais para o aprimoramento dos processos, mas contribuem para a ineficiência dos processos quando são negligenciadas. Essa negligência reduz o moral da equipe e inibe contribuições proativas, deixando ineficiências sem solução.

Esse aspecto relacionado à ineficácia dos _stand-ups_ foi observado em 16 das 24 entrevistas, abrangendo todos os casos. A falta de ação após as retrospectivas foi examinada em 9 entrevistas, abrangendo C1, C2 e C3.

### Organização desestruturada
A organização desestruturada indica dificuldades em organizar os processos de desenvolvimento de LSA de maneira que todas as tarefas sejam executadas de forma contínua e coordenada. Os entrevistados exemplificaram esse problema em relação a tempo, esforço e prazos, aspectos observados em 19 das 24 entrevistas, abrangendo todos os casos.

### Ambiguidade de papéis
Os frameworks ágeis definem papéis com responsabilidades específicas; entretanto, nas empresas participantes do estudo, o envolvimento incompleto com essas responsabilidades — denominado **“ambiguidade de papéis”** — prejudica a eficiência dos processos.

### Prioridades mal definidas
Prioridades mal definidas apareceram em 18 das 24 entrevistas, abrangendo todos os casos, manifestando-se como “sprints às cegas” (C1, C2, C4), comprometimentos da qualidade (todos os casos) e superestimação de tarefas (C1, C2, C3).

A definição inadequada de prioridades ocorre quando o planejamento não possui estimativas precisas de tempo e esforço ou uma priorização clara das tarefas, levando as equipes a iniciar sprints sem objetivos bem definidos. Essa falta de preparação resulta em ineficiências e em falhas frequentes no cumprimento das metas dos sprints, muitas vezes levando as equipes a ignorar protocolos de testes para cumprir os prazos e, consequentemente, comprometer a qualidade.

### Incompatibilidade de habilidades
A incompatibilidade de habilidades foi observada de maneira geral em todas as empresas participantes, especialmente em C4, onde havia carência de engenheiros de telecomunicações. Isso representa uma manifestação específica de domínio de um desafio mais amplo: alinhar as capacidades da força de trabalho às demandas técnicas.

Adequar as habilidades da força de trabalho às necessidades dos projetos é fundamental em organizações orientadas pela tecnologia. Entretanto, as equipes de LSA analisadas apresentam uma incompatibilidade significativa entre habilidades e requisitos do trabalho. Compostas predominantemente por graduados em ciência da computação, essas equipes não possuem a experiência necessária em engenharia de telecomunicações exigida pelo domínio da tecnologia específica.

### Infraestrutura
A infraestrutura — ferramentas, sistemas e hardware — é essencial para o desenvolvimento de software em ambientes de LSA. Os indicadores relacionados à infraestrutura foram mais evidentes em C4 (restrições para testes de hardware) e C2 (problemas na cadeia de ferramentas), aparecendo em 12 das 24 entrevistas.

Isso representa uma restrição crítica, mas frequentemente negligenciada, dos processos, que afeta diretamente o acúmulo de TD.

## Aspectos relacionados às pessoas
O desenvolvimento de software é uma atividade intensiva em conhecimento, que exige tanto conhecimento explícito do domínio quanto conhecimentos adquiridos por meio da experiência. Os aspectos relacionados às pessoas que contribuem para a dívida técnica (TD) surgem de características pessoais, como conhecimento, experiência ou capacidade de adaptação a ambientes de trabalho dinâmicos.

### Falta de conhecimento do domínio
A **falta de conhecimento do domínio** parece ser o principal fator dos desafios relacionados às pessoas, dificultando a cooperação entre equipes em ambientes de LSA. Lacunas de conhecimento do domínio apareceram em 16 das 24 entrevistas, abrangendo todos os casos, manifestando-se tanto como uma compreensão superficial do produto (todos os casos) quanto como uma distribuição desigual de conhecimento especializado (C1, C2, C3). Esse foi o principal fator relacionado às pessoas mencionado pelos participantes. Um líder de equipe destacou o impacto do conhecimento limitado do domínio: “Somos uma equipe completamente nova e não temos muito conhecimento do domínio, mas é interessante porque eles a nova equipe estão muito focados no seu próprio pequeno mundo e não no mundo como um todo. Então, é difícil cooperar com eles como equipe porque, como equipe, você quer utilizar todos, quer que todos trabalhem como uma equipe” (P3).

### Fricções no trabalho em equipe
**Fricções no trabalho em equipe**, manifestadas por comportamentos individuais ou coletivos, como cinismo ou desrespeito, podem prejudicar o moral e a estrutura da equipe, aprofundando ainda mais os desafios relacionados às pessoas. Embora não tenham sido detalhadas extensivamente nas entrevistas, a possibilidade dessas dinâmicas foi sugerida por referências a “reclamações” (P2) e à resistência à educação (P3), indicando que problemas interpessoais não tratados podem ampliar os desafios de colaboração.

### Relutância em atualizar habilidades
A **relutância em atualizar habilidades** apareceu em 8 entrevistas, principalmente envolvendo funcionários com muitos anos de experiência (mais de 10 anos) nos casos C1, C2 e C4. Esse padrão foi menos evidente em C3, que possuía programas mais estruturados de desenvolvimento de competências. A resistência por parte de funcionários experientes foi observada principalmente em C1, C2 e C4.

## Aspectos relacionados à documentação
Em projetos de LSA, nos quais múltiplas equipes gerenciam bases de código complexas, os aspectos relacionados à documentação que contribuem para a TD se acumulam quando os registros não conseguem refletir com precisão as funcionalidades, características e arquitetura em constante evolução do projeto. Isso gera confusão, reduz a velocidade de desenvolvimento e dificulta a manutenção, a escalabilidade e a capacidade de adaptação dos sistemas de software. Em vez de considerar os problemas de documentação como um tipo separado de dívida, analisamos como eles criam condições que levam à necessidade de atalhos e comprometimentos técnicos.

### Baixa qualidade da documentação do sistema
A Tabela 8 apresenta os indicadores dos aspectos relacionados à documentação que contribuem para a TD em ambientes de LSA, destacando seu impacto generalizado nos fluxos de trabalho colaborativos.

Problemas de documentação foram mencionados por 19 dos 24 entrevistados, abrangendo todos os casos. Entretanto, C3 representou uma exceção, apresentando práticas de documentação consideravelmente melhores, atribuídas a uma cultura madura de documentação e à presença de redatores técnicos dedicados.

Uma documentação ineficaz não acompanha as atualizações atuais do sistema ou as mudanças arquiteturais e se torna um obstáculo, especialmente em contextos de LSA, nos quais várias equipes dependem de uma compreensão compartilhada. Registros desatualizados ou incompletos levam a interpretações equivocadas e dificultam a integração de novos membros da equipe, prejudicando a produtividade geral.

A **baixa qualidade da documentação do sistema**, relatada por 15 dos 24 entrevistados nos casos C1, C2 e C4, destacou esse desafio: “Temos uma qualidade muito ruim na documentação sobre como os sistemas são estruturados, como eles executam diferentes funcionalidades e como as diferentes partes dos sistemas, na forma de componentes, estão conectadas entre si” (P6). A documentação contribuindo para a **dívida de qualidade** foi destacada por 14 dos 24 participantes nos casos C1, C2 e C4.

### Documentação do trabalho de outra pessoa
A **documentação do trabalho de outra pessoa**, que frequentemente está fora da área de especialização principal de quem a realiza, tende a ocorrer em projetos de LSA. Isso, combinado com o compartilhamento inadequado de conhecimento, produz registros incompletos ou enganosos, afetando a manutenção e a escalabilidade futuras. Esse indicador apareceu em 10 entrevistas nos casos C1, C2 e C4. Um desenvolvedor comentou: “Às vezes documentamos funcionalidades nas quais não estivemos diretamente envolvidos e acho que isso é menos eficaz devido à falta de uma compreensão mais profunda e de experiência prática.

### Documentação desatualizada
A **documentação desatualizada** afetou os processos de trabalho em todos os casos, sendo mencionada por 17 dos 24 entrevistados. Isso se manifestou tanto na documentação em nível de código (comentários e documentação de APIs) quanto na documentação em nível de sistema (arquitetura e especificações de integração). Por exemplo, documentação de código desatualizada ou inexistente torna os processos de revisão mais lentos, aumenta a recorrência de erros e gera frustração entre os membros da equipe. Um Scrum Master defendeu a adoção de práticas melhores: “Eu realmente quero que todos façam um esforço para comentar o código adequadamente e parem de pegar atalhos na documentação.

### Práticas de documentação desconhecidas
**Práticas de documentação desconhecidas** apareceram em 11 entrevistas nos casos C1, C2 e C4. Isso foi particularmente problemático quando os projetos eram transferidos entre equipes ou consultores, uma vez que a ausência de supervisão centralizada pode resultar em soluções abaixo do ideal e registros fragmentados. As práticas mais formalizadas de C3 novamente representaram uma exceção.

## Aspectos relacionados aos requisitos
Os aspectos relacionados aos requisitos que contribuem para a TD representam um desafio crítico em LSA, caracterizado pela expansão contínua do escopo dos projetos por meio de frequentes adições de funcionalidades e demandas em constante evolução. Esse fenômeno cria um ciclo permanente de mudanças que dificulta a conclusão dos projetos, interrompe fluxos de trabalho estabelecidos e gera ineficiências nas equipes de desenvolvimento.

### Aumento descontrolado do escopo do projeto
O **aumento descontrolado do escopo do projeto (scope creep)** representa o principal fator dos aspectos relacionados aos requisitos que contribuem para a TD e resulta da expansão não controlada do escopo do projeto. As equipes de projeto enfrentam a adição contínua de novos requisitos sem os correspondentes ajustes nos prazos ou nos recursos.

### Requisitos urgentes
**Requisitos urgentes**, impostos pela gestão, apareceram em 16 das 24 entrevistas, principalmente em C1, C2 e C4, onde estruturas hierárquicas tradicionais coexistiam com práticas ágeis. A estrutura mais horizontal de C3 apresentou menos evidências desse padrão.

### Mudanças não planejadas nos requisitos
**Mudanças não planejadas nos requisitos** apareceram em 15 das 24 entrevistas, abrangendo todos os casos. Isso se manifestou por meio de documentação inadequada, discussões insuficientes com as partes interessadas e mecanismos frágeis de priorização para requisitos emergentes.

### Aumento do escopo dos requisitos
O **aumento do escopo dos requisitos** começa com um escopo inicial indefinido, o que leva a projetos sem limites claros. Esse indicador apareceu em 12 entrevistas, principalmente em C1, C2 e C4. O problema foi particularmente significativo em projetos voltados para clientes, nos quais as expectativas dos clientes eram mal gerenciadas, tornando necessária uma comunicação mais assertiva sobre prazos realistas e expectativas de qualidade.

# Discussão
Nosso estudo amplia a compreensão dos aspectos não técnicos que contribuem para a TD em contextos de LSA, demonstrando como eles interagem sistematicamente com a TD.

O conceito de **dívida de requisitos** deve ser compreendido como simultaneamente contínuo e distinto dos desafios clássicos da engenharia de requisitos. Embora nossos resultados demonstrem como esclarecimentos adiados e o aumento do escopo acumulam consequências técnicas em contextos ágeis, esses fenômenos se apoiam em fundamentos da engenharia de requisitos — particularmente estudos sobre volatilidade (Davis, 1993), ambiguidade (Zave e Jackson, 1997a; Zave e Jackson, 1997b) e dificuldades essenciais da especificação de software (Brooks e Bullet, 1987). Os aspectos relacionados aos requisitos em contextos de LSA criam padrões de acúmulo únicos.

Os aspectos relacionados aos requisitos em ambientes de LSA criam uma complexa rede de desafios técnicos, organizacionais e relacionados a processos. Embora a literatura tradicional de engenharia de requisitos tenha documentado extensivamente os desafios de volatilidade e ambiguidade, nossos resultados mostram como a aplicação de métodos ágeis em escala cria novos padrões de acúmulo.

A emergência das **dinâmicas sociais** foi fundamental nesse contexto, com barreiras de comunicação e ambiguidades na tomada de decisões criando condições favoráveis a comprometimentos arquiteturais. Isso amplia o conceito de dívida social ao demonstrar como estruturas de equipes distribuídas em LSA intensificam esses efeitos por meio da redução da comunicação não verbal.


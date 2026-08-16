#engenharia-de-software 

# Contexto
Não é suficiente apenas a presença de desenvolvedores altamente treinados, era necessário um guia organizacional, um processo.

Processo é o conjunto de passos que tem como objetivo atingir uma meta
Processo de software é o processo que visa produzir software de modo eficiente.

# Processo Unificado
É uma abordagem iterativa e incremental para o desenvolvimento de software. Tem foco na arquitetura, fiscos e requisitos, em 1995 foi criado pelos fundadores da UML.
Em 1998 o Processo Unificado (PU) teve o incremento das melhores práticas da Rational tornando-se o RUP, já em 2003 a IBM incorpora a Rational tornando-se o IRUP.

## Filosofia
- Linguagem padrão
- Usa modelos, padrões e guias
- Equipes treinadas
- Ferramentas de apoio

## Ciclo de vida
O RUP repete vários ciclos até a conclusão, cada ciclo gera um artefato (ex: produto liberado para uso). Cada ciclo possui 4 fases e seus marcos (milestones):
- Concepção
- Elaboração
- Construção 
- Transição
Cada fase pode ter várias iterações, que são apresentadas como letras: R(requisitos), A(análise), D(design/projeto), I(implementação) e T(teste), essas letras representam disciplinas técnicas da ES que ocorrem simultaneamente em graus variados.

## Conceitos Relacionados
- Papéis: representado por uma pessoa ou grupo no processo de software
- Comportamento: descreve as atividades que cada papel executa
- Responsabilidade: mostra como os papéis se relaciona com os artefatos, seja criando, modificando ou controlando.
- Relação indivíduo-papel: 
- Atividade: é uma unidade de trabalho que um indivíduo assumindo um papel pode executar e que gera resultado (ex: script de BD, manual, documentos de configuração). As atividades possuem as seguintes atividades:
	- Envolvem criação ou atualização de artefatos
	- São medidas geralmente em horas ou dias
	- Podem variar de pequenas a grandes
	- São atribuídas ao papel

## Boas práticas
- Desenvolvimento iterativo: simplificação de problemas, análise de risco precoce, correção contínua de defeitos
- Gerenciamento de requisitos: identificação como um processo contínuo, identificar, avaliar e acompanhar.
- Arquitetura baseada em componentes: reuso e reutilização
- Modelagem visual (UML)
- Verificação de qualidade: controle contínuo de qualidade, criação de testes em várias iterações.
- Controle de mudanças: manter a rastreabilidade.

## Fases do RUP
![[Pasted image 20260505142118.png]]

### 1 - Iniciação (Concepção)
- Papéis relacionados: Gerentes de projeto, arquitetos e analistas de sistema.
- Objetivos: Análise de viabilidade, Caso de Negócio, Levantamento de Riscos e Requisitos.
- 

### 2 - Elaboração
- Papéis: Gerentes de Projeto, Arquitetos, Analistas de Sistema
- Objetivo: Criar linha-base arquitetural executável
- Artefatos produzidos: Modelo de caso de uso

### 3 - Construção
- Papéis: Desenvolvedores, testadores
- Objetivo: completar os requisitos
- Artefatos produzidos: Modelo de caso de uso
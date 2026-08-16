#MADS

# Introdução
O Android Open Source Project (AOSP) liderado pela Google, serve como base para diversos sistemas Android, como o: Samsung Galaxy, OnePlus, OPPO Find e Honor MagicOS são variantes que estendem o AOSP do Google. Como as variantes do Android desenvolvidas pelos fabricantes e o AOSP são mantidos de forma independente, por diferentes organizações e bases de código, o repositório de uma variante pode ser visto como um fork divergente de logo prazo do AOSP.

Com o lançamento frequente de novas versões do AOSP, os fabricantes precisam realizar atualizações do Android, integrando as mudanças mais recentes do AOSP em suas variantes. Como tanto o AOSP quanto suas variantes passam por modificações extensas, cada atualização do Android envolve de forma inevitável grandes conflitos de merge. 

![[Pasted image 20260319104908.png]]

A pesquisa em si focou na compreensão sobre as atividades relacionadas a conflitos realizadas na prática e nos desafios enfrentados pelos profissionais, realizando uma triangulaçãO metodológica que mostrou que o processo de atualização do Android, é essencialmente, um processo de evolução arquitetural, exigindo um pensamento arquitetural e não apenas correções em nível de código. Especificamente, foram identificados desafios nas seguintes etapas:
- Análise de Baseline: Mudanças na arquitetura dificultam a avaliação de compatibilidade entre AOSP e variantes, a definição da estratégia de atualização e a previsão de qualidade e custo.
- Análise das causas dos conflitos: Modificações invasivas feitas pelas variantes Android na arquitetura AOSP geram muitos conflitos. Problemas de arquitetura e má gestão de branches agravam a situação.
- Resolução de conflitos: Desenvolvedores têm dificuldade em entender a intenção das mudanças no código. Ferramentas automáticas apresentam limitações em precisão, desempenho e usabilidade.
- Análise de impacto: Os conflitos afetam etapas futuras do processo e podem até impactar novas atualizações, devido à propagação por dependências arquiteturais.

Os resultados indicam oportunidades de melhoria na prática de atualização do Android por meio de técnicas de análise de arquitetura de software, que incluem:
- Melhorar documentação da evolução da arquitetura
- Criar modelo Tempo, Qualidade e Custo (TQC) para prever riscos
- Padronizar o gerenciamento de branches
- Investir em refatoração arquitetural para reduzir dependências problemáticas
- Fortalecer a colaboração entre equipes e o compartilhamento de conhecimento

# Resultados e análise
O questionário aplicado durante a pesquisa investigou as etapas envolvidas na resolução manual de conflitos, pelos desenvolvedores. Com base nas respostas foram identificados os seguintes passos:
1. Os desenvolvedores identificam as linhas de código onde ocorre o conflito
2. Realizam o rastreamento do histórico de modificações relacionadas ao conflito, tanto no AOSP quanto na variante para entender a intenção das mudanças no código.
3. Os desenvolvedores pensam em uma solução adequada para resolver o conflito.
4. Eles implementam e verificam a solução.

Devido à falta de familiaridade com os commits do AOSP e da variante em si, os desenvolvedores encontram dificuldade em identificar a intenção por trás das mudanças no código. É feita uma análise na frequência com que os desenvolvedores consultam o histórico de commits do AOSP e das variantes ao resolver conflitos.

Com base nos documentos fornecidos, preparei um roteiro estruturado para a sua apresentação, organizado de forma lógica para cobrir desde o problema central até as possíveis soluções.


---
# Roteiro de Apresentação: Desafios da Evolução Arquitetural no Android
#### 1. Introdução e Contexto

"Olá a todos. Hoje vamos discutir os desafios críticos na manutenção e atualização do sistema operacional Android. Como sabemos, o **Android Open Source Project (AOSP)**, liderado pelo Google, serve como base para diversos dispositivos que usamos, como Samsung Galaxy, OnePlus e outros.

O ponto central aqui é que esses fabricantes criam **variantes** que funcionam como **forks de longo prazo** do AOSP. Como ambas as bases de código (AOSP e a variante do fabricante) evoluem de forma independente e extensa, cada nova versão lançada pelo Google exige uma integração que resulta inevitavelmente em **grandes conflitos de merge**."

#### 2. A Natureza do Problema

"Uma pesquisa aprofundada revelou que o processo de atualização do Android não é apenas uma tarefa de correção de código em nível micro. Na verdade, trata-se de um processo de **evolução arquitetural**.

Isso significa que resolver esses conflitos exige um **pensamento arquitetural** e não apenas ajustes técnicos pontuais. A pesquisa identificou desafios em quatro etapas principais:

- **Análise de Baseline:** A dificuldade em avaliar a compatibilidade e prever custos e qualidade devido a mudanças na arquitetura.
- **Análise das Causas:** Modificações invasivas feitas pelos fabricantes na arquitetura original do AOSP geram conflitos complexos.
- **Resolução de Conflitos:** A dificuldade de entender a 'intenção' das mudanças originais e a limitação das ferramentas automáticas.
- **Análise de Impacto:** Como esses conflitos se propagam por dependências e afetam futuras atualizações."

#### 3. O Fluxo de Trabalho do Desenvolvedor

"Para entendermos o lado prático, a pesquisa mapeou como os desenvolvedores resolvem esses conflitos manualmente:

1. Primeiro, identificam as linhas exatas do conflito.
2. Em seguida, realizam um **rastreamento do histórico** tanto no AOSP quanto na variante para tentar entender por que aquele código foi alterado.
3. Só então eles pensam em uma solução adequada, implementam e verificam.

O maior obstáculo aqui é a **falta de familiaridade** com os commits. Muitas vezes, o desenvolvedor não sabe qual era a intenção original da mudança, o que torna a resolução lenta e propensa a erros."

#### 4. Oportunidades de Melhoria e Conclusão

"Finalmente, os resultados da pesquisa apontam caminhos claros para melhorar essa prática através da análise de arquitetura de software:

- **Documentação:** Precisamos de registros melhores sobre como a arquitetura está evoluindo.
- **Previsibilidade:** Criar modelos que considerem **Tempo, Qualidade e Custo (TQC)** para prever riscos antes de iniciar a atualização.
- **Padronização e Refatoração:** Investir em refatoração arquitetural para reduzir dependências problemáticas e padronizar o gerenciamento de branches.
- **Colaboração:** Fortalecer a troca de conhecimento entre as equipes.

Em resumo, para otimizar as atualizações do Android, devemos parar de olhar apenas para as linhas de código e começar a focar na **integridade da arquitetura do software**."

---

**Dica para a apresentação:** Você pode utilizar os quatro passos do fluxo de trabalho do desenvolvedor (item 3) para ilustrar o "dia a dia" da dor do desenvolvedor, contrastando com as melhorias sugeridas (item 4) como o caminho para o futuro.
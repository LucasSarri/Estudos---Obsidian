
# 1 - Introduction
Os testes de software aumentam a confiança na correção de um programa, existindo diversas abordagens para medir a qualidade dos testes. A **análise de mutação** (_mutation analysis_) é uma dessas abordagens e vem sendo cada vez mais adotada pela indústria, evidenciando a necessidade de que engenheiros de software aprendam técnicas de análise de mutação e testes.

Entretanto, estudantes de Engenharia de Software e Ciência da Computação enfrentam desafios ao aprender técnicas de teste novas e complexas. Diante disso, os autores buscaram compreender melhor os desafios e as implicações de infraestrutura envolvidos no ensino da análise de mutação em ambientes educacionais.

O uso da análise e do teste de mutação em contextos educacionais já foi estudado anteriormente, incluindo o desenvolvimento de módulos educacionais específicos, abordagens gamificadas para ensino e o uso da análise de mutação para fornecer feedback sobre a qualidade dos conjuntos de testes produzidos pelos estudantes. Apesar dessas contribuições, os autores destacam que ainda não havia estudos investigando as vantagens e desvantagens de diferentes ferramentas de análise de mutação sob a perspectiva de professores e alunos.

# 3 - Experimental Setup
Esta seção descreve a metodologia utilizada em comum tanto no **Estudo de Scaffolding** quanto no **Estudo de Visualização**. Em particular, são apresentados os programas utilizados nos experimentos, as ferramentas de análise de mutação empregadas e as métricas avaliadas. Aspectos específicos de cada estudo são discutidos posteriormente em suas respectivas seções.

Ambos os estudos foram organizados em duas fases:

- **Primeira fase:** observação dos desafios enfrentados pelos estudantes durante a realização dos exercícios de teste de mutação, funcionando como grupo de controle;
- **Segunda fase:** implementação de soluções para os desafios identificados e repetição do mesmo exercício de teste de mutação.

## 3.1 - Programas utilizados

### Triangle
O **Triangle** é um programa Java autocontido amplamente utilizado para fins educacionais. Ele recebe como entrada três números inteiros que representam os comprimentos dos lados de um triângulo e retorna sua classificação:

- Equilátero;
- Escaleno;
- Isósceles;
- Inválido.

O framework de mutação **Major** inclui o programa Triangle como exemplo oficial.

Os autores escolheram esse programa porque ele possui:

- Código relativamente curto;
- Especificação intuitiva e fácil de compreender;
- Fluxo de controle não trivial, permitindo a criação de casos de teste mais elaborados.

### DateUtils
O **DateUtils** faz parte do projeto **Lang** e fornece funções utilitárias para manipulação de objetos Java dos tipos **Calendar** e **Date**.

### HelpFormatter
O **HelpFormatter** pertence ao projeto **Cli** e é responsável pela formatação de mensagens de ajuda utilizadas em aplicações de linha de comando.

### JsonWriter
O **JsonWriter** integra o projeto **Gson** e oferece funcionalidades para escrita de dados JSON em fluxos (_streams_).



# Resumo
Essa lacuna de conhecimento impede que pesquisadores identifiquem novas oportunidades de pesquisa, que desenvolvedores de ferramentas invistam em automações realmente necessárias, que mantenedores de bibliotecas tomem decisões informadas sobre novas versões e que programadores adotem práticas adequadas ao utilizar bibliotecas de ML.

Este estudo apresenta a primeira pesquisa empírica de larga escala, quantitativa e qualitativa, destinada a compreender como os desenvolvedores utilizam bibliotecas de Machine Learning no contexto do Software 2.0 e como a evolução dessas bibliotecas impacta o código-fonte.

## Principais resultados

Foi identificado um crescimento expressivo no uso de bibliotecas de ML:

- A proporção de novos projetos Python que utilizavam bibliotecas de Machine Learning aumentou de **2% em 2013 para 50% em 2018**.

Também foram observados diversos padrões de uso:

1. **36% dos projetos utilizam múltiplas bibliotecas de ML** para implementar diferentes etapas do fluxo de trabalho de Machine Learning.
2. Os desenvolvedores **atualizam bibliotecas de ML com maior frequência** do que bibliotecas tradicionais de software.
3. Atualizações do tipo **strict upgrade** (atualizações rigorosas para versões específicas mais recentes) são as mais comuns entre as bibliotecas de ML.
4. Atualizações em bibliotecas de ML frequentemente desencadeiam **atualizações em cascata** de outras dependências do projeto.
5. Bibliotecas de ML também são frequentemente **rebaixadas para versões anteriores (downgrade)**, ocorrendo em aproximadamente **22,04% dos casos analisados**.

## Desafios específicos do Software 2.0

O estudo identificou desafios que são pouco comuns em softwares tradicionais, mas frequentes em aplicações baseadas em Machine Learning:

- **Incompatibilidade binária de modelos treinados**, onde modelos gerados por uma versão da biblioteca podem não funcionar corretamente em versões posteriores.
- **Dificuldade de benchmark e comparação de modelos de ML**, tornando mais complexo avaliar se uma atualização realmente melhora o desempenho do sistema.

## Contribuições do estudo

Por fim, os autores apresentam recomendações práticas para diferentes públicos envolvidos no ecossistema de Software 2.0, incluindo:

- Pesquisadores;
- Desenvolvedores de ferramentas;
- Engenheiros de software;
- Educadores;
- Mantenedores e fornecedores de bibliotecas;
- Fabricantes de hardware.

Essas recomendações visam facilitar a evolução, manutenção e adoção de sistemas baseados em Machine Learning, contribuindo para o desenvolvimento de softwares mais robustos e sustentáveis ao longo do tempo.

# Metodologia de Pesquisa
Neste estudo, os autores utilizam métodos **quantitativos e qualitativos** para responder a seis questões de pesquisa.

Primeiramente, foi realizada uma análise estática de um conjunto de **18.122 projetos Python hospedados no GitHub**. Em seguida, foi conduzido um estudo longitudinal sobre o histórico de commits de **3.340 projetos identificados como aplicações de Software 2.0**.

Além disso, foi conduzido um estudo qualitativo por meio de uma pesquisa com **477 desenvolvedores** que haviam introduzido ou atualizado bibliotecas de Machine Learning em projetos pertencentes ao conjunto analisado.

A análise quantitativa teve como objetivo compreender:

- Como os desenvolvedores utilizam bibliotecas de Machine Learning;
- Como esse uso evolui ao longo do ciclo de vida dos projetos.

Já o estudo qualitativo buscou identificar:

- As motivações para introduzir bibliotecas de ML;
- Os desafios enfrentados durante sua adoção e atualização.

## Sistemas Analisados

### Principais Projetos Python do GitHub
O conjunto de dados utilizado contém **18.122 projetos Python populares e de grande porte hospedados no GitHub**.

O processo de seleção dos projetos foi inspirado no trabalho de Yu et al. [142], que investigou o uso de anotações Java em projetos reais.

Os autores selecionaram todos os repositórios que atendiam aos seguintes critérios:

- Escrito em Python;
- Não ser um fork;
- Não estar arquivado;
- Possuir mais de **50 estrelas (stargazers)** até 31 de dezembro de 2018.

Para evitar a inclusão de projetos inativos, foram descartados os repositórios que não apresentaram nenhuma atividade nos seis meses anteriores à coleta dos dados (31 de dezembro de 2018).

Além disso, seguindo recomendações de estudos anteriores, os autores também excluíram projetos com menos de **três contribuidores**, focando apenas em projetos efetivamente ativos e colaborativos.

Após a aplicação desses critérios, o conjunto final totalizou **18.122 repositórios**.

### Bibliotecas de ML
Machine Learning (ML) é suportado por diversas bibliotecas populares. Braiek et al. identificaram sete bibliotecas de ML populares mantidas por empresas e oito mantidas pela comunidade, todas baseadas em Python. Enquanto pesquisas anteriores concentraram-se principalmente nas seis bibliotecas mais populares — TensorFlow, Scikit-learn, Keras, PyTorch, Caffe e Theano — os autores deste estudo identificaram todos os projetos clientes dessas 15 bibliotecas em seu conjunto de dados, conforme mostrado na Tabela 1.

Os resultados mostraram que **95% dos projetos analisados utilizam uma das seis bibliotecas mais populares**. Por esse motivo, o restante do artigo concentra a análise nos projetos que utilizam essas seis bibliotecas, referindo-se a elas simplesmente como **“bibliotecas de ML”**.

## Análise Estática do Código-Fonte
Os autores analisaram a versão mais recente de cada projeto do conjunto de dados para identificar os clientes das bibliotecas de ML e compreender como essas bibliotecas são utilizadas.

### Identificação de Aplicações Software 2.0
Para estudar a evolução do uso de bibliotecas de ML em aplicações **Software 2.0**, era necessário identificar os projetos que realmente utilizavam essas bibliotecas.

Os pesquisadores analisaram as principais versões das bibliotecas de ML e coletaram todos os nomes de seus pacotes-raiz. Para determinar se um projeto utilizava uma biblioteca de ML, verificaram dois critérios:
1. O projeto continha instruções de importação (`import`) que apontavam para os pacotes-raiz da biblioteca.
2. O projeto realizava pelo menos uma chamada de API da biblioteca de ML.

Com base nesses critérios, foram identificados **3.340 projetos** que utilizavam uma das seis bibliotecas de ML selecionadas. A lista completa dos projetos foi disponibilizada em um site complementar ao artigo.

### Análise do Uso das APIs
Os autores aprofundaram a análise desses 3.340 projetos para entender como os desenvolvedores utilizam as APIs fornecidas pelas bibliotecas de ML.

Para isso, identificaram:

- Chamadas de métodos das bibliotecas.
- Referências a objetos vinculados a essas bibliotecas.

Entretanto, existe um desafio importante: **Python é uma linguagem dinamicamente tipada**, o que significa que muitas informações sobre tipos só estão disponíveis durante a execução do programa.

Executar todos os 3.340 projetos para coletar essas informações seria inviável. Para contornar esse problema, os pesquisadores utilizaram ferramentas de análise estática capazes de inferir tipos sem executar o código.

Entre elas:

- Jedi
- MyPy

O **MyPy** exige que o código utilize anotações de tipo (introduzidas no Python 3.5). No entanto, **93,88% dos projetos analisados não utilizavam essas anotações**, tornando o MyPy inadequado para o estudo.

Já o **Jedi** consegue inferir informações de tipos utilizando apenas o código-fonte e as dependências externas do projeto. Além disso, trata-se de uma ferramenta bastante popular e já utilizada em pesquisas anteriores.

Por esses motivos, os autores escolheram o **Jedi** para inferir as informações de vinculação de tipos necessárias à análise.


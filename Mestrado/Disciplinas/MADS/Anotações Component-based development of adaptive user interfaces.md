# Resumo
Interfaces de Usuário modernas (**UIs**) são cada vez mais esperadas como **plásticas**, no sentido de manterem um nível constante de **usabilidade**, mesmo quando submetidas a mudanças de contexto em tempo de execução.

As **Interfaces de Usuário Adaptativas (AUIs)** têm sido propostas como uma solução para a variabilidade de contexto, devido à sua capacidade de **se adaptar automaticamente ao contexto de uso em tempo real**.

No entanto, o desenvolvimento de AUIs é uma tarefa complexa, pois diferentes aspectos precisam ser considerados, como:

- **monitoramento de contexto**
- **adaptação da interface**

Em trabalhos anteriores, abordagens baseadas em **engenharia dirigida por modelos (model-driven engineering)** foram propostas para apoiar o desenvolvimento de AUIs de forma sistemática e eficiente.

Entretanto, essas abordagens ainda enfrentam desafios relacionados a:

- **flexibilidade**
- **reutilização**
- **compatibilidade com frameworks padrão de mercado**, como o **Angular**

Essas limitações dificultam sua adoção na indústria.

Para resolver esse problema e explorar uma alternativa, propomos um **framework de desenvolvimento baseado em componentes para AUIs**, chamado **CoBAUI**.

O **CoBAUI** define um framework modular para apoiar o desenvolvimento de AUIs e é composto por diversos componentes que cobrem aspectos como:

- **monitoramento de contexto**
- **adaptação da interface no nível de widgets**

O framework CoBAUI foi implementado com base no **Angular** e tem como objetivo apoiar o desenvolvimento de AUIs por meio de componentes **altamente reutilizáveis e flexíveis**.

Demonstramos os benefícios do framework CoBAUI por meio de um **estudo de caso**, envolvendo uma AUI para uma **aplicação web de biblioteca**.

# Introdução
Para garantir a funcionalidade e a usabilidade das interfaces de usuário em diferentes dispositivos é preciso considerar o contexto. Neste sentido as Interfaces de Usuário Adaptativas (AUIs) têm sido propostas como uma solução para essa variabilidade de contextos, pois conseguem se adpatar a mudança de contexto em tempo de execução.
Porém o desenvolvimento de AUIs é complexo e exige alto esforço, para isso surgiram abordagens baseadas em model-driven (engenharia dirigida por modelos) para tentar reduzir o esforço, porém usando essas abordagens ainda se mantiveram problemas relacionados a flexibilidade, reutilização e padronização, assim dificultando sua adoção pela indústria.
Para lidar com essas limitações o estudo apresenta um framework para desenvolvimento de interfaces adaptativas baseado em componentes, ele é inspirado no framework teórico COMET, o nome do framework desenvolvido é CoBAUI (Component-Based Framework for Adaptive UIs) que foi implementado com base no Angular.

# O Framework CoBAUI
No desenvolvimento de interfaces baseado em componentes (CBUID), as interfaces são compostas por componentes individuais, sendo que cada componente contribui para o objetivo geral de interação.
O CBUID busca reduzir a complexidade do desenvolvimento de interfaces por meio de reutilização e modularização. Partes da interface dousuário e suas funcionalidades associadas são encapsuladas em componentes e só podem ser acessadas por meio de interfaces bem definidas.
![[Pasted image 20260408170318.png|697]]
O framework CoBAUI segue o princípio de separação de responsabilidades, com o objetivo de desacoplar as diferentes responsabilidades de uma interface adaptativa, que são:
- Captura de contexto (Context Capturing)
- Tomada de decisão (Decision Making)
- Lógica de adaptação (Adpatation Logic)

Na imagem abaixo é apresentada a arquitetura baseada em componentes para uma interface adaptativa.
![[Pasted image 20260408170836.png]]
Cada área de responsabilidade é tratada por um tipo específico de componente, sendo que cada componente possuí uma função bem definida, atua de forma isolada e desacoplada, e segue o princípio de responsabilidade única.

Para atender esses requisitos, foram identificados quatro tipos principais de componentes:
- Provedor de Contexto (Context Provider)
- Provedor de Regras (Rule Provider)
- Avaliador de Regras (Rule Evaluator)
- Widget Adaptativa (Adaptive Widget)

Além disso, há um componente central chamado Adaptation Controller, que atua como conector permitindo a comunicação e colaboração entre todos os componentes, tornando a interface coesa
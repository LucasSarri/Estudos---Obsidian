#MADS 

# Linguagem da Conexão: Interface
Regra de ouro do DBC: as interações ocorrem apenas através de interfaces públicas e conhecidas, descritas por operações parametrizadas.

- Interface requerida (required): Define os serviços e dependências que devem estar disponíveis no ambiente hospedeiro para que 

# Estudo de caso: Componente coletor de dados
- Interface requires: sensorManagement, sensorData.
- Interface provides: sensorData, removeSensor, startSensor, stopSensor, testSensor, initialise, report e listAll.

# Espectro da reutilização
A materialização do DBC em uma organização se divide em três abordagens complementares.
- Desenvolvimento COM reuso: compor o novo sistema aproveitando peças já existentes. Especialmente útil para componentes do domínio de negócio da própria organização.
- Desenvolvimento PARA reuso: projetar e construir sistemas focando na criação de novos componentes robustos que alimentarão o catálogo da empresa no futuro.
- Componentes Prontos (COTS - Commercial Off-The-Shelf): aquisição de componentes a partir de catálogos de terceiros, incluindo compras comerciais ou adoção de software livre.

# Desafio COTS: a realidade da integração
Componentes reutilizados ou de terceiros quase nunca atendem exatamente e perfeitamente aos requisitos do seu sistema. Integrar não é mágica, é negociação.

## Soluções de engenharia
- Adaptar os Requisitos: Modificar o que o negócio espera do sistema para se adequar ao que o componente oferece

# Validação de componentes
- Fase 1 & 2: listar componentes candidatos disponíveis e selecionar o mais promissor.
- Fase 3: validar o componente selecionado sob 3 óticas, requisitos funcionais, atributos de qualidade e restrições do projeto

O componente só é considerado validado após passar por todas as etapas de filtragem, garantindo integridade arquitetural e conformidade com o projeto.

# Panorama metodológico do DBC
A engenharia de software consolidou diversas metodologias formais para guiar o DBC, como UML Components, Catalysis e KobrA.

- Especificação: especificar conjunto de requisitos
- Refinamento: refinar e modificar requisitos com base nos componentes efetivamente disponíveis
- Projeto arquitetural: projetar a arquitetura e buscar componentes simultaneamente
- Composição: Desenvolver compondo os componentes finais.

# Matriz de Trade-offs
## Benefícios
- Redução de custos e tempo de desenvolvimento
- Gerenciamento e redução da complexidade e riscos do sistema
- Desenvolvimento paralelo acelerado graças à decomposição estrutural
- Qualidade superior via uso de componentes previamente


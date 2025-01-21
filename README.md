# Sistema-de-Gerenciamento-de-Estagios
Repositório para atividade final de engenharia de requisitos
## Objetivo do Sistema

O **Sistema de Gerenciamento de Estágios** tem como objetivo proporcionar uma plataforma integrada e eficiente que conecta estudantes, empresas e instituições de ensino, facilitando o gerenciamento e a busca de oportunidades de estágio. A proposta é otimizar o processo seletivo, promovendo maior agilidade e transparência na contratação de estagiários, além de proporcionar aos estudantes uma experiência simplificada e segura no acompanhamento de suas candidaturas e progresso nas seleções.

Com o sistema, buscamos resolver os seguintes desafios:

- **Para os estudantes:** Facilitar a busca de vagas adequadas às suas áreas de interesse, possibilitando o gerenciamento de candidaturas e o acompanhamento em tempo real do status de cada processo seletivo.
- **Para as empresas:** Proporcionar uma plataforma centralizada para a publicação de vagas de estágio, facilitando a busca de candidatos qualificados e o gerenciamento de todo o processo seletivo.
- **Para as instituições de ensino:** Oferecer uma maneira eficiente de monitorar o progresso dos alunos durante o estágio e manter uma comunicação constante com empresas e estudantes.

O sistema visa, assim, aumentar a eficiência no processo de busca e contratação de estagiários, contribuir para o desenvolvimento dos estudantes e oferecer uma gestão mais eficaz e centralizada das vagas de estágio.

## Padrão para Desenvolvimento

O desenvolvimento do **Sistema de Gerenciamento de Estágios** seguirá uma abordagem estruturada e baseada nas melhores práticas de engenharia de software, garantindo que o sistema seja escalável, seguro, de fácil manutenção e com uma boa experiência para o usuário final. As principais diretrizes a serem seguidas incluem:

### Organização

Com o objetivo de manter uma pradonização e organização durante o desenvolvimento
Em necessidade de adicionar qualquer formato de anexo para auxiliar na documentação deve se utiliza o acesso ao drive: https://drive.google.com/drive/folders/1yvKWzYXwISeYyp9kHS9IEQxDOrVxDFj3?usp=sharing

### Metodologia Ágil (Scrum)
O desenvolvimento será conduzido utilizando a metodologia ágil **Scrum**, permitindo entregas contínuas e feedback constante dos stakeholders. O trabalho será dividido em sprints, e as funcionalidades serão desenvolvidas de forma iterativa, priorizando as mais críticas para o sucesso do sistema.

### Arquitetura do Sistema
A arquitetura do sistema será baseada no padrão **MVC (Model-View-Controller)**, garantindo uma separação clara entre a lógica de negócios, a interface de usuário e a manipulação de dados. Além disso, o sistema será orientado a **microserviços** para maior escalabilidade e flexibilidade na manutenção e adição de novas funcionalidades.


### Requisitos

#### Estrutura de Diretórios

Os artefatos de requisitos serão organizados dentro do diretório principal `Requisitos`, com as seguintes subcategorias e subpastas específicas:

- **Requisitos Funcionais**:  
   - Diretório principal: `Documentação/Requisitos/Funcionais/`  
   - Subpastas para os tipos de requisitos funcionais:
     -  Cadastro - `Documentação/Requisitos/Funcionais/Cadastro/`  
     -  Busca - `Documentação/Requisitos/Funcionais/Busca/`  
     -  Painel - `Documentação/Requisitos/Funcionais/Painel/`  
     -  Sistema - `Documentação/Requisitos/Funcionais/Sistema/`  
     -  Integração - `Documentação/Requisitos/Funcionais/Integracao/`  
     -  Filtro - `Documentação/Requisitos/Funcionais/Filtro/`  
     - Acompanhamento - `Documentação/Requisitos/Funcionais/Acompanhamento/`  
     -  Autenticação - `Documentação/Requisitos/Funcionais/Autenticacao/`  

- **Requisitos Legais**:  
   - Diretório principal: `Documentação/Requisitos/Legais/`

- **Requisitos Não Funcionais**:  
   - Diretório principal: `Documentação/Requisitos/NaoFuncionais/`  
   - Subpastas para os tipos de requisitos não funcionais:
     -  Escalabilidade - `Documentação/Requisitos/NaoFuncionais/Escalabilidade/`  
     -  Segurança - `Documentação/Requisitos/NaoFuncionais/Seguranca/`  
     -  Integridade - `Documentação/Requisitos/NaoFuncionais/Integridade/`  
     -  Performance - `Documentação/Requisitos/NaoFuncionais/Performance/`  
     -  Usabilidade - `Documentação/Requisitos/NaoFuncionais/Usabilidade/`  
     -  Interoperabilidade - `Documentação/Requisitos/NaoFuncionais/Interoperabilidade/`  
     -  Privacidade - `Documentação/Requisitos/NaoFuncionais/Privacidade/`  

---


#### Nomeclatura dos Requisitos Funcionais
Os requisitos funcionais são identificados como RF, seguidos de uma categoria para facilitar a organização:

- C: Cadastro - Relacionados ao cadastro de informações dos usuários e vagas.
- B: Busca - Relacionados à pesquisa de vagas de estágio.
- P: Painel - Relacionados às funcionalidades disponíveis nos paineis do estudante e da empresa.
- S: Sistema - Relacionados às funcionalidades gerais do sistema.
- I: Integração - Relacionados à integração do sistema com outras plataformas ou serviços.
- F: Filtro - Relacionados à aplicação de filtros nas buscas.
- AC: Acompanhamento - Relacionados ao monitoramento do processo seletivo.
- AU: Autenticação - Relacionados à autenticação de usuários.

Cada requisito funcional é identificado por um código único, que combina a categoria e um número sequencial (por exemplo, `RF-C001` para o primeiro requisito de cadastro).

#### Nomeclatura dos Requisitos Não Funcionais    

Os requisitos não funcionais são identificados como RNF, seguidos de uma categoria para facilitar a organização:

- ESC: Escalabilidade - Relacionados à capacidade dinâmica e estática do sistema.
- SEG: Segurança - Relacionados ao controle de acesso, comunicação segura e proteção de dados.
- INT: Integridade - Relacionados à preservação e consistência dos dados.
- PERF: Performance - Relacionados ao tempo de resposta e eficiência do sistema.
- USAB: Usabilidade - Relacionados à facilidade de uso e aprendizado do sistema.
- INTEROP: Interoperabilidade - Relacionados à integração do sistema com outros sistemas e formatos de dados.
- PRIV: Privacidade - Relacionados ao controle de acesso e visibilidade das informações sensíveis.

Cada requisito não funcional é identificado por um código único, que combina a categoria e um número sequencial (por exemplo, `RNF-ESC01` para o primeiro requisito de escalabilidade).


#### Organização

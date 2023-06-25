# 							Documento de Requisitos



| Data de alteração | Versão |      Descrição       | Responsável |
| :---------------: | :----: | :------------------: | :---------: |
|     23/06/23      |  1.0   | Criação do documento |   Adriano   |



##  1. Descrição do software

### 1.1  Justificativa

   Visando garantir a segurança em condomínios o acesso de veículos é bem restrito, sendo necessário o preenchimento de registros e outros vários processos burocráticos para a autorização da entrada. Assim, a entrega de comida/objetos ou mesmo a entrada de funcionários de aplicativos de corrida pode ficar demorada e complexa. Assim, o uso de um software que deixe o processo mais rápido, sem comprometer a segurança do condomínio, se faz necessária.

### 1.2   Objetivo

   Associar a detecção da placa do veículo aos dados em um banco de dados referente aos veículos autorizados a entrar no condomínio para que o acesso dele seja mais rápido e fácil.

### 1.3  Benefícios

- Agilidade na entrada do condomínio
- Maior controle sobre o fluxo de visitantes e entregadores
- Automatização do processo

### 1.4 Descrição

Um aplicativo que permita aos funcionários consultar informações sobre moradores e visitantes e verificar o fluxo de entrada de automóveis e no qual os moradores possam permitir o acesso de visitantes de forma automática.

### 1.5 Principais Requisitos:

- Cadastro de visitantes
- Consulta no banco de dados dos usuários cadastrados por parte do funcionário
- Registro e consulta de eventos de entrada no condomínio
- Permitir ao morador alterar seus dados e cadastrar novos automóveis



## 2. Requisitos Funcionais (RF)



| Código | Requisito                                    | Descrição                                                    |
| ------ | -------------------------------------------- | ------------------------------------------------------------ |
| RF01   | Autenticação                                 | Os usuários devem ser capazes de fazer login no sistema com seus dados de acesso |
| RF02   | Cadastro de visitantes                       | O morador deve ser capaz de cadastrar/remover um visitante (temporário) no banco de dados |
| RF03   | Consultar visitantes                         | O morador deve ser capaz de consultar as informações relativas aos visitantes vinculados ao seu usuário |
| RF04   | Alterar dados pessoais                       | O morador deve ser capaz de alterar seus dados pessoais      |
| RF05   | Consultar acessos de visitantes pelo morador | O morador deve ser capaz de consultar os acessos mais recentes de visitantes vinculados ao seu usuário |
| RF06   | Buscar morador                               | O funcionário autorizado deve ser capaz de buscar as informações de um morador |
| RF07   | Listar moradores                             | O funcionário autorizado deve ser capaz de visualizar a lista de moradores cadastrados |
| RF08   | Logs do sistema                              | O funcionário autorizado deve ser capaz de visualizar todos os eventos de tentativa de entrada |



## Requisitos Não Funcionais (RNF)

| Código | Requisito                         | Descrição                                                    |
| ------ | --------------------------------- | ------------------------------------------------------------ |
| RNF01  | Criptografia de dados             | Criptografia de todos os dados pessoais                      |
| RNF02  | Grupos de acesso                  | Restringir funcionalidades de acordo com o tipo de usuário   |
| RNF03  | Protocolos Seguros de Comunicação | Protocolos criptografados como HTTPS, SSH, etc.              |
| RNF04  | Banco de Dados                    | O banco de dados deve ser construído utilizando SQL          |
| RNF05  | Plataforma                        | Os usuários devem ser capazes de acessar pelo celular ou desktop |

# Sprint2-JavaAdvanced - ExperienceIA

![Java](https://img.shields.io/badge/Java-007396?style=flat&logo=java&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat&logo=spring&logoColor=white)
![RESTful](https://img.shields.io/badge/RESTful-02569B?style=flat&logo=restful&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat&logo=hibernate&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

# Atualizações da Sprint1 para a Sprint2

Na transição da Sprint1 para a Sprint2, o projeto Java Advanced - ExperienceIA passou por diversas melhorias e expansões significativas. A seguir, detalhamos as principais atualizações e adições que foram implementadas:

## 1. Novos Arquivos Criados

### 1.1. Controllers Adicionados

- **AvaliacaoController.java**: Gerencia operações CRUD (Create, Read, Update, Delete) relacionadas às avaliações dos usuários.
- **LoginController.java**: Responsável pelo gerenciamento das operações de login, permitindo a criação, atualização, consulta e deleção de registros de login.
- **TrendController.java**: Administra as operações sobre tendências, incluindo a criação, atualização, consulta e deleção de dados sobre tendências de mercado ou usuário.
- **FeedbackController.java**: Encapsula as operações relacionadas ao feedback dos usuários, permitindo a coleta e gestão de opiniões e avaliações fornecidas pelos usuários.

### 1.2. DTOs Adicionados

- **AvaliacaoDto.java**: Data Transfer Object para transferir dados relacionados às avaliações entre as camadas da aplicação.
- **LoginDto.java**: Data Transfer Object que facilita a transferência de dados de login entre as camadas do sistema.

### 1.3. Entidades Adicionadas

- **Avaliacao.java**: Representa a entidade de avaliação, incluindo atributos como nota, feedback e cliente.
- **Login.java**: Define a entidade de login com atributos como ID, email e senha.
- **Trend.java**: Entidade que representa uma tendência, contendo informações como tópico, frequência e sentimentos associados.
- **Feedback.java**: Entidade que captura feedbacks dos usuários, incluindo descrição, data de criação e sentimento.

### 1.4. Repositories Adicionados

- **AvaliacaoRepository.java**: Repositório para realizar operações CRUD na base de dados relacionadas às avaliações.
- **LoginRepository.java**: Repositório para gerenciamento dos dados de login no banco de dados.
- **TrendRepository.java**: Repositório que facilita a interação com a base de dados para operações relacionadas às tendências.
- **FeedbackRepository.java**: Repositório dedicado à manipulação dos dados de feedback na base de dados.

### 1.5. Services Adicionados

- **AvaliacaoService.java**: Serviço que contém a lógica de negócio para gerenciar avaliações, garantindo a aplicação das regras de negócio adequadas.
- **LoginService.java**: Serviço que encapsula a lógica de negócio relacionada aos logins, incluindo autenticação e gestão de credenciais.
- **TrendService.java**: Serviço responsável por aplicar as regras de negócio no gerenciamento de tendências.
- **FeedbackService.java**: Serviço que gerencia a lógica de negócio para a coleta e processamento de feedbacks dos usuários.

## 2. Atualizações nos Arquivos Existentes

### 2.1. ClienteService.java

- Adição do método **atualizarParcialmente**, que permite atualizações parciais de um cliente utilizando reflexão para modificar dinamicamente os campos especificados.

### 2.2. ClienteController.java

- Inclusão de novos métodos HTTP:
  - **PATCH**: Permite atualizações parciais nos dados dos clientes.
  - **OPTIONS**: Verifica os métodos HTTP disponíveis para um recurso específico.
  - **HEAD**: Verifica a existência de um recurso sem retornar o corpo da resposta.

### 2.3. Cliente.java

- Limpeza do código com a remoção de linhas em branco desnecessárias, mantendo a consistência e legibilidade do código.

## Conclusão

As atualizações da Sprint2 expandiram significativamente o escopo e a funcionalidade do projeto, introduzindo novos componentes para gerenciar avaliações, logins, tendências e feedbacks. Esses novos elementos não só aumentam a capacidade do sistema de lidar com diferentes tipos de dados e operações, mas também melhoram a flexibilidade e a eficiência do gerenciamento de informações. As melhorias no gerenciamento de clientes, com a adição de métodos de atualização parcial e verificação de métodos disponíveis, demonstram um avanço na maturidade e sofisticação do projeto, tornando-o mais robusto e preparado para atender às necessidades dos usuários e do mercado.

## Equipe de Desenvolvimento

- **Gabriel Jesus** - *Entidades e JPA/Hibernate*
  - Implementação das classes de entidade
  - Configuração do framework Hibernate e JPA

- **Rafael Lino** - *API RESTful e Modelagem de Dados*
  - Desenvolvimento dos endpoints RESTful
  - Adoção do modelo de maturidade de Richardson para APIs

- **Bruno Antunes** - *Gestão de Configuração e Versões*
  - Gerenciamento de artefatos de software
  - Controle de versões usando Git

- **Gabriel Henrique** - *Testes e Validação*
  - Criação e execução de testes dos endpoints
  - Produção de vídeo demonstrativo dos testes

- **Pedro Ferrari** - *Comunicação e Apresentação*
  - Desenvolvimento do vídeo de apresentação do projeto
  - Elaboração e configuração dos slides e demais recursos visuais

## Vídeos

### Vídeo de Apresentação da Ideia Principal
[![Vídeo de Apresentação](http://img.youtube.com/vi/rii3foLBHkw/0.jpg)](https://youtu.be/rii3foLBHkw "Vídeo de Apresentação da Ideia Principal - Clique e Assista!")

### Demonstração dos Endpoints
[![Demonstração dos Endpoints](http://img.youtube.com/vi/Fm6A2inDUq4/0.jpg)](https://youtu.be/Fm6A2inDUq4 "Demonstração dos Endpoints - Clique e Assista!")

## Como Rodar a Aplicação

### Pré-requisitos

Antes de executar a aplicação, certifique-se de que o seguinte software está instalado:

- **Java JDK 11** ou superior: Necessário para executar a aplicação Java.
- **IntelliJ IDEA** ou **Eclipse**: IDEs recomendadas para este projeto.

### Instruções de Execução Usando IntelliJ IDEA

1. **Abrir o Projeto**:
   - Inicie o IntelliJ IDEA e selecione "Open" ou "Import Project".
   - Navegue até o diretório onde o projeto foi clonado e selecione o arquivo `pom.xml`. Clique em "Open as Project".

2. **Configurar o JDK**:
   - Vá em `File` > `Project Structure` > `Project`.
   - No campo "Project SDK", selecione o Java JDK 11 (ou versão superior que você instalou).
   - Clique em "Apply" e depois "OK".

3. **Executar a Aplicação**:
   - Localize a classe principal que contém o método `main` chamada `ExpericeIaApplication`.
   - Clique com o botão direito do mouse sobre o arquivo e selecione "Run 'ExpericeIaApplication.main()'".
   - O IntelliJ IDEA irá compilar e executar a aplicação. O servidor embutido (como Tomcat ou Jetty) será iniciado e a aplicação ficará acessível através de `localhost:8080`.

### Instruções de Execução Usando Eclipse

1. **Importar o Projeto**:
   - Inicie o Eclipse e vá em `File` > `Import` > `Maven` > `Existing Maven Projects`.
   - Navegue até o diretório onde o projeto foi clonado e selecione a pasta contendo o `pom.xml`. Clique em "Finish".

2. **Configurar o JDK**:
   - Clique com o botão direito do mouse sobre o projeto no "Package Explorer" e selecione `Build Path` > `Configure Build Path`.
   - Na aba "Libraries", clique em "Add Library", selecione "JRE System Library", escolha "Next", então "Workspace Default JRE" (deve ser ajustado para JDK 11 ou superior) e clique "Finish".

3. **Executar a Aplicação**:
   - Encontre a classe principal que contém o método `main` na view "Package Explorer".
   - Clique com o botão direito sobre ela e selecione "Run As" > "Java Application".
   - Eclipse irá compilar e executar a aplicação. O servidor embutido será iniciado e a aplicação estará disponível em `localhost:8080`.

## Acessando a Aplicação

Após iniciar a aplicação, você pode acessar `localhost:8080` em qualquer navegador web para interagir com a interface da aplicação ou usar clientes de API como Postman para acessar os endpoints RESTful conforme documentados.

## Documentação da API

### Endpoints Disponíveis

## Endpoints de Clientes
- **Listar Todos os Clientes**
  - `GET /usuarios`
  - **Descrição:** Retorna uma lista de todos os clientes.
  - **URL de Requisição:** `localhost:8080/usuarios`

- **Criar Cliente**
  - `POST /usuarios`
  - **Descrição:** Adiciona um novo cliente.
  - **Corpo da Requisição:**
    ```json
    {
      "telefone": "123456",
      "email": "cliente@gmail.com",
      "cnpj": "3347516508",
      "nome": "Cliente",
      "tipoEmpresa": "varejo"
    }
    ```
  - **URL de Requisição:** `localhost:8080/usuarios`

- **Atualizar Cliente**
  - `PUT /usuarios/{id}`
  - **Descrição:** Atualiza os dados de um cliente específico.
  - **Parâmetros de URL:** `id` - ID do cliente a ser atualizado.
  - **Corpo da Requisição:**
    ```json
    {
      "telefone": "987654",
      "email": "clientenovo@gmail.com",
      "cnpj": "3347516508",
      "nome": "Cliente Novo",
      "tipoEmpresa": "varejo"
    }
    ```
  - **URL de Requisição:** `localhost:8080/usuarios/{id}`

- **Deletar Cliente**
  - `DELETE /usuarios/{id}`
  - **Descrição:** Remove um cliente com base no ID fornecido.
  - **Parâmetros de URL:** `id` - ID do cliente a ser removido.
  - **URL de Requisição:** `localhost:8080/usuarios/{id}`

- **Consultar Cliente por ID**
  - `GET /usuarios/{id}`
  - **Descrição:** Retorna os detalhes de um cliente específico.
  - **Parâmetros de URL:** `id` - ID do cliente.
  - **URL de Requisição:** `localhost:8080/usuarios/{id}`

- **Atualizar Parcialmente Cliente**
  - `PATCH /usuarios/{id}`
  - **Descrição:** Atualiza parcialmente os dados de um cliente específico.
  - **Parâmetros de URL:** `id` - ID do cliente a ser atualizado.
  - **Corpo da Requisição:** 
    ```json
    {
      "telefone": "987654"
    }
    ```
  - **URL de Requisição:** `localhost:8080/usuarios/{id}`

- **Verificar Disponibilidade de Métodos**
  - `OPTIONS /usuarios/{id}`
  - **Descrição:** Verifica os métodos disponíveis para um recurso específico.
  - **Parâmetros de URL:** `id` - ID do cliente.
  - **URL de Requisição:** `localhost:8080/usuarios/{id}`

- **Consultar Cliente (HEAD)**
  - `HEAD /usuarios/{id}`
  - **Descrição:** Verifica a existência de um cliente sem retornar o corpo.
  - **Parâmetros de URL:** `id` - ID do cliente.
  - **URL de Requisição:** `localhost:8080/usuarios/{id}`

## Endpoints de Avaliações
- **Listar Todas as Avaliações**
  - `GET /avaliacoes`
  - **Descrição:** Retorna uma lista de todas as avaliações.
  - **URL de Requisição:** `localhost:8080/resultado`

- **Criar Avaliação**
  - `POST /avaliacoes`
  - **Descrição:** Adiciona uma nova avaliação.
  - **Corpo da Requisição:**
    ```json
    {
      "avaliacaoNota": 10,
      "avaliacaoFeedback": "Excelente serviço",
    }
    ```
  - **URL de Requisição:** `localhost:8080/resultado`

- **Atualizar Avaliação**
  - `PUT /resultado/{id}`
  - **Descrição:** Atualiza os dados de uma avaliação específica.
  - **Parâmetros de URL:** `id` - ID da avaliação a ser atualizada.
  - **Corpo da Requisição:**
    ```json
    {
      "avaliacaoNota": 9,
      "avaliacaoFeedback": "Bom serviço",
    }
    ```
  - **URL de Requisição:** `localhost:8080/resultado/{id}`

- **Deletar Avaliação**
  - `DELETE /avaliacoes/{id}`
  - **Descrição:** Remove uma avaliação com base no ID fornecido.
  - **Parâmetros de URL:** `id` - ID da avaliação a ser removida.
  - **URL de Requisição:** `localhost:8080/avaliacoes/{id}`

- **Consultar Avaliação por ID**
  - `GET /resultado/{id}`
  - **Descrição:** Retorna os detalhes de uma avaliação específica.
  - **Parâmetros de URL:** `id` - ID da avaliação.
  - **URL de Requisição:** `localhost:8080/resultado/{id}`

## Endpoints de Logins
- **Listar Todos os Logins**
  - `GET /logins`
  - **Descrição:** Retorna uma lista de todos os logins.
  - **URL de Requisição:** `localhost:8080/logins`

- **Criar Login**
  - `POST /logins`
  - **Descrição:** Adiciona um novo login.
  - **Corpo da Requisição:**
    ```json
    {
      "emailLogin": "usuario1@example.com",
      "senhaLogin": "senha123"
    }
    ```
  - **URL de Requisição:** `localhost:8080/logins`

- **Atualizar Login**
  - `PUT /logins/{id}`
  - **Descrição:** Atualiza os dados de um login específico.
  - **Parâmetros de URL:** `id` - ID do login a ser atualizado.
  - **Corpo da Requisição:**
    ```json
    {
      "emailLogin": "usuario1@example.com",
      "senhaLogin": "novaSenha123"
    }
    ```
  - **URL de Requisição:** `localhost:8080/logins/{id}`

- **Deletar Login**
  - `DELETE /logins/{id}`
  - **Descrição:** Remove um login com base no ID fornecido.
  - **Parâmetros de URL:** `id` - ID do login a ser removido.
  - **URL de Requisição:** `localhost:8080/logins/{id}`

- **Consultar Login por ID**
  - `GET /logins/{id}`
  - **Descrição:** Retorna os detalhes de um login específico.
  - **Parâmetros de URL:** `id` - ID do login.
  - **URL de Requisição:** `localhost:8080/logins/{id}`

## Endpoints de Tendências
- **Listar Todas as Tendências**
  - `GET /tendencias`
  - **Descrição:** Retorna uma lista de todas as tendências.
  - **URL de Requisição:** `localhost:8080/tendencias`

- **Criar Tendência**
  - `POST /trends`
  - **Descrição:** Adiciona uma nova tendência.
  - **Corpo da Requisição:**
    ```json
    {
      "topico": "Tendência 1",
      "frequencia": 100,
      "sentimentoPositivo": 80.0,
      "sentimentoNeutro": 15.0,
      "sentimentoNegativo": 5.0,
      "dataInicio": "2024-01-01",
      "dataFim": "2024-01-31"
    }
    ```
  - **URL de Requisição:** `localhost:8080/trends`

- **Atualizar Tendência**
  - `PUT /trends/{id}`
  - **Descrição:** Atualiza os dados de uma tendência específica.
  - **Parâmetros de URL:** `id` - ID da tendência a ser atualizada.
  - **Corpo da Requisição:**
    ```json
    {
      "topico": "Tendência 1 Atualizada",
      "frequencia": 120,
      "sentimentoPositivo": 85.0,
      "sentimentoNeutro": 10.0,
      "sentimentoNegativo": 5.0,
      "dataInicio": "2024-01-01",
      "dataFim": "2024-01-31"
    }
    ```
  - **URL de Requisição:** `localhost:8080/trends/{id}`

- **Deletar Tendência**
  - `DELETE /tendencias/{id}`
  - **Descrição:** Remove uma tendência com base no ID fornecido.
  - **Parâmetros de URL:** `id` - ID da tendência a ser removida.
  - **URL de Requisição:** `localhost:8080/trends/{id}`

- **Consultar Tendência por ID**
  - `GET /tendencias/{id}`
  - **Descrição:** Retorna os detalhes de uma tendência específica.
  - **Parâmetros de URL:** `id` - ID da tendência.
  - **URL de Requisição:** `localhost:8080/trends/{id}`
 
 ## Endpoints de Feedback
- **Listar Todos os Feedbacks**
  - `GET /feedbacks`
  - **Descrição:** Retorna uma lista de todos os feedbacks.
  - **URL de Requisição:** `localhost:8080/feedbacks`

- **Criar Feedback**
  - `POST /feedbacks`
  - **Descrição:** Adiciona um novo feedback.
  - **Corpo da Requisição:**
    ```json
    { 
      "descricao": "Ótimo atendimento",
      "dataCriacao": "2024-01-01",
      "sentimento": "positivo"
    }
    ```
  - **URL de Requisição:** `localhost:8080/feedbacks`

- **Atualizar Feedback**
  - `PUT /feedbacks/{id}`
  - **Descrição:** Atualiza os dados de um feedback específico.
  - **Parâmetros de URL:** `id` - ID do feedback a ser atualizado.
  - **Corpo da Requisição:**
    ```json
    { 
      "descricao": "Atendimento bom",
      "dataCriacao": "2024-01-01",
      "sentimento": "neutro"
    }
    ```
  - **URL de Requisição:** `localhost:8080/feedbacks/{id}`

- **Deletar Feedback**
  - `DELETE /feedbacks/{id}`
  - **Descrição:** Remove um feedback com base no ID fornecido.
  - **Parâmetros de URL:** `id` - ID do feedback a ser removido.
  - **URL de Requisição:** `localhost:8080/feedbacks/{id}`

- **Consultar Feedback por ID**
  - `GET /feedbacks/{id}`
  - **Descrição:** Retorna os detalhes de um feedback específico.
  - **Parâmetros de URL:** `id` - ID do feedback.
  - **URL de Requisição:** `localhost:8080/feedbacks/{id}`

## Cronograma de Desenvolvimento

| Atividade                               | Responsável       |  Data de Conclusão  |
|-----------------------------------------|-------------------|---------------------|
| Implementação das Classes de Entidade   | Gabriel Jesus     | 19/05/2024          |
| Criação dos Endpoints RESTful           | Rafael Lino       | 17/05/2024          |
| Configuração de Artefatos               | Bruno Antunes     | 20/05/2024          |
| Criação do Vídeo de Testes              | Gabriel Henrique  | 15/05/2024          |
| Criação do Vídeo de Apresentação        | Pedro Ferrari     | 18/05/2024          |

## Diagramas

### Diagrama de Classes
![Diagrama de Classes](https://raw.githubusercontent.com/bruno1098/Sprint1-JavaAdvanced/main/Images/DiagramaClasses.png)

### Diagrama Lógico
![Diagrama Lógico](https://raw.githubusercontent.com/bruno1098/Sprint1-JavaAdvanced/main/Images/WhatsApp%20Image%202024-04-15%20at%2020.14.27.jpeg?raw=true)

### Diagrama Relacional
![Diagrama Relacional](https://raw.githubusercontent.com/bruno1098/Sprint1-JavaAdvanced/main/Images/WhatsApp%20Image%202024-04-15%20at%2020.14.28.jpeg?raw=true)

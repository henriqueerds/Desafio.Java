# Voll.med - Aplicação de Clínica Médica

Voll.med é uma aplicação Java desenvolvida com o framework Spring Boot para gerenciar uma clínica médica. Esta aplicação oferece funcionalidades para cadastrar médicos, pacientes, agendar consultas, cancelar consultas e detalhar informações relevantes. Ela utiliza um banco de dados MySQL para armazenar os dados dos pacientes, médicos e consultas, além de segurança com tokens JWT para autenticação.

## Funcionalidades

A aplicação possui as seguintes funcionalidades:

- **Cadastro de Médicos**: Os médicos podem ser cadastrados com informações como nome, especialidade, e outros dados relevantes.

- **Cadastro de Pacientes**: Os pacientes podem ser cadastrados com informações como nome, data de nascimento, e outros detalhes.

- **Agendamento de Consultas**: Os pacientes podem agendar consultas médicas, especificando o médico, data e hora da consulta.

- **Cancelamento de Consultas**: Consultas agendadas podem ser canceladas, com um motivo associado ao cancelamento.

- **Detalhamento de Informações**: É possível obter detalhes sobre médicos, pacientes e consultas por meio de endpoints dedicados.

- **Autenticação com Token JWT**: Para acessar as funcionalidades protegidas, os usuários devem se autenticar e receber um token JWT.

## Tecnologias Utilizadas

- Java
- Spring Boot
- Spring Data JPA
- MySQL
- Spring Security
- Token JWT
- Swagger UI (documentação da API)
- Lombok (para simplificar a criação de classes)
- Flyway (para migrações de banco de dados)

## Configuração

Certifique-se de configurar corretamente o banco de dados MySQL e as propriedades no arquivo `application.properties` antes de executar a aplicação.

```properties
spring.datasource.url=jdbc:mysql://localhost/vollmed_api
spring.datasource.username=root
spring.datasource.password=senha_do_banco_de_dados
````
Você também pode configurar outras propriedades relacionadas à segurança e ao token JWT neste arquivo.

## Executando a Aplicação
Para executar a aplicação, você pode usar o comando Maven:
```
mvn spring-boot:run
```
Após a inicialização bem-sucedida, você pode acessar a documentação da API usando o Swagger UI em http://localhost:8080/swagger-ui.html.

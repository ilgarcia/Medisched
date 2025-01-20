# Medisched

> Mockup de um projeto utilizando Java e Nest.js

## Funcionalidades Principais

### Para Pacientes:

1. Cadastro de Pacientes

* Registro de dados básicos (nome, e-mail, telefone, endereço).
* Possibilidade de criar uma conta com autenticação JWT.

2. Agendamento de Consultas

* Seleção de médicos disponíveis por especialidade.
* Escolha de horários livres.
* Cancelamento de consultas com notificação automática.

### Para Médicos:

1. Gestão de Agenda

* Visualização e edição dos horários disponíveis.
* Recebimento de notificações sobre consultas marcadas ou canceladas.

2. Consulta de Histórico Médico

* Acesso ao histórico de consultas dos pacientes (somente médicos autorizados).

### Para Administradores:

1. Gestão Geral

* CRUD completo de pacientes, médicos e horários de atendimento.
* Relatórios com estatísticas (número de consultas realizadas, horários mais procurados, etc.).

2. Gestão de Especialidades Médicas

* Cadastro e atribuição de especialidades aos médicos.

## Arquitetura do Projeto

### Backend em Java (Spring Boot)

* O backend será responsável por gerenciar as regras de negócio e fornecer uma API para o Nest.js.
Banco de dados relacional com MySQL.
* Autenticação JWT ou OAuth2.

### API Gateway com Nest.js

* Usar Nest.js para criar uma camada de comunicação com o backend Java.
* Implementar GraphQL ou REST para facilitar o acesso às funcionalidades.
* Utilizar validações com decorators (ex.: @IsEmail, @Length) do Nest.js.

### Banco de Dados

* MongoDB para o Nest.js, caso use cache ou outros dados rápidos.
* MySQL integrado com o backend Java para dados críticos.

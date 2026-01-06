# MedCare — Sistema de Agendamento de Consultas Médicas

## 📌 Visão Geral

O **MedCare** é um sistema de **agendamento e gestão de consultas médicas**, desenvolvido em **Java**, seguindo o padrão de arquitetura **MVC (Model–View–Controller)** e utilizando **DAO** para acesso a dados. O sistema permite o cadastro de médicos e pacientes, bem como o agendamento, listagem e gerenciamento de consultas médicas.

Este projeto é voltado para fins **acadêmicos**, sendo ideal para demonstrar boas práticas de organização, separação de responsabilidades e integração com banco de dados.

---

## 🗂️ Estrutura do Projeto

```text
├── README.md
├── SistemaConsultasMedicas
│   ├── SistemaConsultasMedicas.iml
│   └── src
│       └── project
│           ├── Main.java
│           ├── controller
│           │   ├── ConsultaController.java
│           │   ├── MedicoController.java
│           │   └── PacienteController.java
│           ├── dao
│           │   ├── Conexao.java
│           │   ├── ConsultaDAO.java
│           │   ├── MedicoDAO.java
│           │   └── PacienteDAO.java
│           ├── model
│           │   ├── Consulta.java
│           │   ├── Medico.java
│           │   └── Paciente.java
│           └── view
│               ├── AgendarConsulta.java
│               ├── CadastroMedico.java
│               ├── CadastroPaciente.java
│               ├── ListarConsulta.java
│               ├── ListarMedicos.java
│               ├── ListarPacientes.java
│               ├── TestaConexao.java
│               └── TestaDAO.java
└── bancodedados.zip
```

---

## 🧱 Arquitetura MVC

### 🔹 Model

Responsável pela representação das entidades do sistema:

* `Paciente`
* `Medico`
* `Consulta`

Cada classe modela os dados e regras de negócio básicas.

---

### 🔹 DAO (Data Access Object)

Camada responsável pela comunicação com o banco de dados.

* `Conexao` → gerencia a conexão com o banco
* `PacienteDAO`
* `MedicoDAO`
* `ConsultaDAO`

Essa camada garante isolamento entre regras de negócio e persistência de dados.

---

### 🔹 Controller

Responsável por intermediar as ações do usuário entre a **View** e o **Model**.

* `PacienteController`
* `MedicoController`
* `ConsultaController`

---

### 🔹 View

Interfaces gráficas desenvolvidas em **Java Swing**, responsáveis pela interação com o usuário.

Funcionalidades disponíveis:

* Cadastro de pacientes
* Cadastro de médicos
* Agendamento de consultas
* Listagem de médicos, pacientes e consultas

---

## ▶️ Execução do Projeto

1. Importe o projeto em uma IDE Java (ex: **NetBeans** ou **IntelliJ IDEA**)
2. Configure o banco de dados utilizando o arquivo `bancodedados.zip`
3. Ajuste as credenciais no arquivo `Conexao.java`
4. Execute a classe `Main.java`

---

## 🎯 Funcionalidades

* Cadastro de médicos
* Cadastro de pacientes
* Agendamento de consultas
* Listagem e controle de consultas
* Testes de conexão e DAO

---

## 🚀 Possíveis Melhorias Futuras

* Validação avançada de dados
* Relatórios em PDF
* Autenticaç

# 🧪 QA Automation Project - E2E Burger

Projeto de automação de testes web utilizando **Java, Selenium WebDriver e JUnit 5**, aplicando o padrão **Page Object Model (POM)**.

Os testes automatizados validam o fluxo de **cadastro de usuários** no sistema E2E Burger, considerando diferentes perfis de acesso.

---

## 🌐 Sistema testado

E2E Burger  
https://e2eburguer.netlify.app/

Aplicação web com fluxo de cadastro para dois tipos de usuário:

- Gestor (Gestão)
- Cliente (Salão)

---

## 🎯 Objetivo do projeto

Validar o comportamento do formulário de cadastro, garantindo que:

- os campos obrigatórios sejam preenchidos corretamente
- a senha atenda aos critérios de segurança
- a confirmação de senha funcione corretamente
- o usuário consiga se cadastrar como Gestor ou Cliente
- o sistema aceite o cadastro com dados válidos

---

## 🧪 Cenários automatizados

### Cadastro positivo - Gestor
Valida que um usuário pode se cadastrar selecionando o perfil **Gestão**.

### Cadastro positivo - Cliente
Valida que um usuário pode se cadastrar selecionando o perfil **Salão**.

---

## 🔐 Regra de senha validada

O sistema exige senha com:

- pelo menos 1 letra maiúscula
- pelo menos 1 caractere especial
- mínimo de 6 caracteres

---

## 🧾 Massa de teste utilizada

Para evitar erro de usuário já cadastrado, foi utilizada geração dinâmica de email.

### Cadastro - Gestor
Nome: Alefe Gestor  
Email: gestor + System.currentTimeMillis() + @gmail.com  
Senha: Teste@123  
Perfil: Gestão  

---

### Cadastro - Cliente
Nome: Cliente Teste  
Email: cliente + System.currentTimeMillis() + @gmail.com  
Senha: Teste@123  
Perfil: Salão  

---

Exemplo de email gerado durante execução:

gestor1713639201345@gmail.com
cliente1713639204521@gmail.com
---

Observação:

O email é gerado dinamicamente para evitar duplicidade:

teste + System.currentTimeMillis() + @gmail.com

## 🧰 Tecnologias utilizadas

- Java 17
- Selenium WebDriver
- JUnit 5
- Maven
- WebDriverManager
- Page Object Model (POM)



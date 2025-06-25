# 💸 Java Bank

![Java](https://img.shields.io/badge/Java-21-blue?style=flat-square)
![Gradle](https://img.shields.io/badge/Gradle-green?style=flat-square)

> Sistema bancário de linha de comando (CLI) desenvolvido em Java 21, com suporte a operações bancárias, Pix, investimentos e auditoria de transações.  
> Criado para praticar conceitos de **Orientação a Objetos**, **tratamento de exceções** e **boas práticas de arquitetura**.

> Projeto desenvolvido inicialmente como parte do bootcamp da [DIO](https://web.dio.me/), com fins educacionais e foco em boas práticas com Java.

---

## 🚀 Funcionalidades

- 📌 Criação de contas com múltiplas chaves Pix  
- 💵 Depósito, saque e transferências entre contas  
- 📈 Cadastro e atualização de investimentos  
- 🧾 Criação de carteiras de investimento associadas às contas  
- 📊 Auditoria com histórico de transações detalhado  
- 🛡️ Tratamento robusto de exceções (conta não encontrada, saldo insuficiente, etc.)

---

## 🛠️ Tecnologias Utilizadas

- Java 21
- Gradle
- Programação Orientada a Objetos (POO)
- Repository Pattern
- Exceções personalizadas

---

## 📁 Estrutura do Projeto

```
src/
└─ main/
    └─ java/
        └─ br/com/dio/
            ├─ Main.java
            ├─ exception/
            │   └─ Exceções específicas.
            ├─ model/
            │   └─ Entidades: Conta, Carteira, Investimento, etc.
            └─ repository/
                └─ Camada de persistência.
```

---

## ⚙️ Como Executar

1. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/java-bank.git
cd java-bank
```

2. **Compile o projeto:**

```bash
./gradlew build
```

3. **Execute a aplicação:**

```bash
./gradlew run
```

---

## 🧩 Fluxo da Aplicação (via terminal)

Ao iniciar a aplicação, o usuário poderá interagir com o seguinte menu:

1. **Criar uma conta** – Informar múltiplas chaves Pix e valor inicial  
2. **Criar um investimento** – Definir taxa de rendimento e valor inicial  
3. **Criar uma carteira de investimento** – Vincular uma conta a um investimento  
4. **Depositar na conta** – Usar chave Pix para realizar depósito  
5. **Sacar da conta** – Usar chave Pix para saque com validação de saldo  
6. **Transferência entre contas** – Usar Pix de origem e destino para enviar dinheiro  
7. **Investir** – Aplicar valores da conta em uma carteira de investimento  
8. **Sacar investimento** – Resgatar valor da carteira de volta para a conta  
9. **Listar contas** – Exibir todas as contas cadastradas  
10. **Listar investimentos** – Exibir todos os investimentos criados  
11. **Listar carteiras de investimento** – Exibir carteiras vinculadas às contas  
12. **Atualizar investimentos** – Reajustar automaticamente os saldos das carteiras  
13. **Histórico de compra** – Exibir extrato de movimentações por Pix  
14. **Sair** – Finaliza a execução da aplicação

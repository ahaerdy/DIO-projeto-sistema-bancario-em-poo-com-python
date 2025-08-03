# DIO-projeto-sistema-bancario-em-poo-com-python

Projeto em Python que implementa um sistema bancário utilizando **Programação Orientada a Objetos (POO)**, com classes abstratas, herança e encapsulamento. Atividade prática dos vídeos 01 e 02 do curso “Modelando o Sistema Bancário em POO com Python” da plataforma [DIO](https://web.dio.me).

## 📚 Curso

- Curso: "Modelando o Sistema Bancário em POO com Python"
- **Instrutor**: Guilherme Arthur de Carvalho (Analista de Sistemas)   
  - [LinkedIn](https://www.linkedin.com/in/decarvalhogui/)
- Repositório de estudos geral: [Bootcamp Suzano Python Developer](https://github.com/ahaerdy/DIO-learning/tree/main/Suzano%20-%20Python%20Developer)

---

## 🎯 Objetivo

Refatorar o sistema bancário inicial, substituindo estruturas baseadas em dicionários por uma modelagem completa com classes e objetos. O desafio é dividido em duas partes:

- **Parte 1**: Criar a estrutura das classes do sistema (Cliente, Conta, ContaCorrente, Histórico, Saque, Depósito etc.).
- **Parte 2**: Integrar a lógica das operações do menu a essas classes, encapsulando o comportamento de saque, depósito, extrato, criação de usuários e contas.

---

## 🛠️ Funcionalidades Implementadas

- ✅ Cadastro de clientes (com validação de CPF único)
- ✅ Criação de contas para clientes
- ✅ Realização de depósitos e saques com regras de negócio
- ✅ Visualização de extrato por conta
- ✅ Registro de transações com data, tipo e valor
- ✅ Controle de limite de saques diários
- ✅ Menu interativo via terminal

---

## 🧱 Estrutura de Classes

- `Cliente` (classe base)
- `PessoaFisica` (herda de Cliente)
- `Conta` (classe base com métodos `sacar`, `depositar`)
- `ContaCorrente` (herda de Conta, com limites)
- `Transacao` (classe abstrata)
- `Saque` e `Deposito` (herdam de Transacao)
- `Historico` (registra as transações)

---

## 🖥️ Tecnologias Utilizadas

- Python 3.10+
- Programação Orientada a Objetos (POO)
- Classes Abstratas (`abc`)
- Encapsulamento e Herança
- Manipulação de listas e entrada de dados via `input`
- `textwrap` para menu interativo

---

## 📁 Arquivos

- `modelo_parte_1.py`: Código com a modelagem das classes (Parte 1 do desafio)
- `modelo_parte_2.py`: Código com menu funcional e integração completa (Parte 2 do desafio)
- `README.md`: Este arquivo explicativo

---

## ▶️ Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/ahaerdy/DIO-projeto-sistema-bancario-em-poo-com-python.git
cd DIO-projeto-sistema-bancario-em-poo-com-python
```

2. Execute o script da parte 2 (completo):

```bash
python modelo_parte_2.py
```

3. Interaja com o sistema via terminal.

## ✅ Regras de Negócio

- Cada cliente possui CPF único
- Cliente pode ter mais de uma conta
- Conta com limite de R$500 por saque
- Máximo de 3 saques por dia
- Todas as operações registradas no histórico da conta

## 📌 Aprendizados

- Aplicação prática de herança e polimorfismo
- Uso de classes abstratas com @abstractmethod
- Encapsulamento de lógica de negócios
- Estruturação de um sistema completo com POO em Python
- Clareza na separação de responsabilidades entre entidades

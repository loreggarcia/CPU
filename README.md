# CPU 8 bits - Arquitetura Simplificada

## 📌 Sobre o projeto

Este projeto consiste na implementação de uma **CPU de 8 bits com arquitetura simplificada**, desenvolvida utilizando o simulador Digital.

A CPU é capaz de executar operações aritméticas básicas e gerenciar ciclos de execução por meio de um circuito de controle.

O projeto foi desenvolvido com base nos requisitos propostos na atividade acadêmica :contentReference[oaicite:0]{index=0}, que incluem:

- Implementação de uma ALU funcional
- Criação de um circuito de controle (fetch + execute)
- Uso de memória para armazenar instruções

---

## 🧠 Arquitetura da CPU

A CPU é composta pelos seguintes módulos:

### 🔹 Program Counter (PC)
Responsável por gerar o endereço da próxima instrução.

### 🔹 Memória (ROM)
Armazena as instruções da CPU.

### 🔹 Instruction Register (IR)
Armazena temporariamente a instrução atual.

### 🔹 ALU (Unidade Lógica e Aritmética)
Executa operações sobre os dados.

### 🔹 Registradores
- **AC (Acumulador)** → armazena resultados das operações
- **MQ (Multiplicação/Quociente)** → utilizado em multiplicação e divisão

### 🔹 Unidade de Controle
Gerencia os ciclos de execução da CPU (fetch e execute).

---

## ⚙️ Operações da ALU

A ALU implementa as seguintes operações :contentReference[oaicite:1]{index=1}:

| Operação | Descrição |
|--------|----------|
| Soma | AC + N |
| Subtração | AC - N |
| Multiplicação | AC * N → AC (LSB) e MQ (MSB) |
| Divisão | AC / N → AC (resto) e MQ (quociente) |
| Shift Left | Deslocamento lógico à esquerda |
| Shift Right | Deslocamento lógico à direita |
| XOR | Operação XOR |
| NAND | Operação NAND |

---

## 🔁 Funcionamento da CPU

### 📥 Ciclo de Busca (Fetch)
1. PC gera o endereço
2. ROM retorna a instrução
3. IR armazena a instrução

### ⚙️ Ciclo de Execução (Execute)
1. Instrução é decodificada
2. ALU executa operação
3. Resultado é armazenado em AC ou MQ

---

## 🧾 Formato da instrução

Cada instrução possui:

- **3 bits de opcode**
- **8 bits de dado**

---

## 🎥 Vídeo de apresentação

> Inserir aqui o link do vídeo do YouTube

---

## 🛠️ Ferramentas utilizadas

- Digital Simulator :contentReference[oaicite:2]{index=2}
- GitHub

---

## 📌 Considerações finais

Este projeto demonstra a construção de uma CPU funcional baseada em princípios fundamentais de arquitetura de computadores, incluindo:

- Separação entre controle e execução
- Uso de registradores e barramentos
- Sequenciamento por clock

---

## 👩‍💻 Autora

Lorena Gabriela

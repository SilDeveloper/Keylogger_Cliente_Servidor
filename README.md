# Estudo de Comunicação Cliente-Servidor via Sockets 🌐

Este projeto consiste em uma implementação de um sistema de monitoramento de eventos de teclado (Keylogger) utilizando a arquitetura **Cliente-Servidor**. Desenvolvido por Silvia e Raphael, para fins estritamente didáticos da UFF, o objetivo é explorar a comunicação em rede e o tratamento de fluxos de dados em tempo real.

## 🛠️ Tecnologias e Bibliotecas
* **Linguagem:** Python
* **Comunicação:** Biblioteca `socket` (TCP/IP)
* **Monitoramento:** `keyboard` (Captura de eventos de I/O)

## 🏗️ Arquitetura do Projeto
O sistema é dividido em dois módulos principais:

1. **Módulo Cliente:**
   * Responsável por capturar as entradas de teclado localmente.
   * Estabelece uma conexão via Socket TCP com o servidor remoto.
   * Transmite os dados capturados de forma contínua.

2. **Módulo Servidor:**
   * Permanece em estado de escuta (*listen*) em uma porta específica.
   * Recebe e armazena os dados enviados pelo cliente.
   * Gerencia múltiplas conexões ou logs de sessão.

---

## ⚠️ Nota de Ética e Segurança
Este repositório é um **PoC (Proof of Concept)** criado para o estudo de Segurança da Informação e Redes de Computadores. 
* O uso deste código em sistemas sem autorização expressa é ilegal e antiético.
* Desenvolvido para demonstrar vulnerabilidades e reforçar a importância de práticas de proteção de endpoint.

## 🚀 Como Executar (Ambiente de Teste)
1. Inicie o servidor para aguardar conexões:
   ```bash
   python servidor.py

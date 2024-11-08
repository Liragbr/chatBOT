﻿# Terminal ChatBot
Esse é o meu primeiro projeto em Python. Analisei alguns fóruns e documentos antes de começá-lo. De início, eu pretendia fazê-lo em C#, mas achei mais interessante dar prosseguimento em Python. Este projeto é uma ferramenta interativa que utiliza a API Groq para processar e responder a consultas do usuário em um ambiente de terminal. Além disso, o chatbot mantém um histórico de conversas para revisão posterior. Este README explica como configurar, utilizar e estender a aplicação.

## Sumário
1. [Visão Geral](#visao-geral)
2. [Funcionalidades](#funcionalidades)
3. [Tecnologias Utilizadas](#tecnologias-utilizadas)
4. [Instalação](#instalacao)
5. [Fluxo de Trabalho Detalhado](#fluxo-de-trabalho-detalhado)

## Visão Geral
O Terminal ChatBot facilita a comunicação com o serviço Groq, permitindo:
1. **Conectar-se ao Serviço Groq**: Estabelece uma conexão com a API Groq.
2. **Enviar Solicitações**: Processa consultas do usuário e retorna respostas.
3. **Salvar e Carregar Histórico de Conversas**: Mantém um registro das interações para consultas futuras.

## Funcionalidades
- **Conexão com a API Groq**: Conecta-se ao serviço Groq para processamento de consultas.
- **Envio de Consultas**: Envia consultas do usuário para o serviço Groq e retorna respostas.
- **Manutenção de Histórico**: Salva e carrega histórico de conversas em um arquivo local.
- **Limpeza de Histórico**: Permite a remoção do histórico de conversas.

## Tecnologias Utilizadas
- **Python**: Linguagem de programação principal para o desenvolvimento da aplicação.
- **requests**: Biblioteca para realizar requisições HTTP.
- **os**: Biblioteca para operações do sistema.
- **datetime**: Biblioteca para manipulação de datas e horas.
- **groq**: Biblioteca para integração com a API Groq.

## Instalação
Para configurar o projeto localmente, siga estas etapas:

1. **Clone o repositório**:
```git clone https://github.com/your-username/TerminalChatBot.git```
2. **Navegue até o diretório do projeto**:
```cd TerminalChatBot```
3. **Instale as bibliotecas necessárias: Utilize o pip para instalar as dependências**:
```pip install requests groq```

## Fluxo de Trabalho Detalhado
### 1. Conexão com a API Groq
A classe GroqConnector gerencia a conexão com a API Groq, utilizando o cliente Groq para estabelecer e verificar a conexão.

### 2. Envio de Consultas
A função send_request dentro da classe GroqConnector envia consultas dos usuários para o serviço Groq e retorna as respostas processadas.

## 3. Manutenção de Histórico
A classe ConversationHistory gerencia o salvamento e a carga do histórico de conversas, facilitando a revisão e limpeza do histórico conforme necessário.


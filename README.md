# 💬 Live Chat em Tempo Real com WebSocket

Aplicação de chat em tempo real desenvolvida com Java + Spring Boot utilizando WebSocket, STOMP e SockJS para comunicação instantânea entre usuários.

O projeto permite conexão em tempo real entre múltiplos clientes, envio de mensagens ao vivo e atualização automática da interface sem necessidade de recarregar a página.

---

# 🚀 Funcionalidades

## 💬 Chat em tempo real

* Envio instantâneo de mensagens
* Atualização automática do chat
* Comunicação bidirecional
* Múltiplos usuários conectados simultaneamente

## 🔌 WebSocket

* Comunicação persistente entre cliente e servidor
* Uso de protocolo STOMP
* Suporte a SockJS

## 🎨 Interface

* Layout moderno e responsivo
* Interface estilizada com CSS
* Mensagens exibidas dinamicamente
* Controle de conexão/desconexão

## 🔒 Segurança básica

* Escape de HTML nas mensagens
* Proteção contra injeção de scripts (XSS)

---

# 🛠 Tecnologias Utilizadas

* Java
* Spring Boot
* Spring WebSocket
* STOMP Protocol
* SockJS
* HTML5
* CSS3
* JavaScript
* jQuery
* Bootstrap

---

# 📂 Estrutura do Projeto

```bash id="82mdk1"
config/
 └── WebSocketConfig

controller/
 └── ChatController

DTOs/
 ├── ChatInputDTO
 └── ChatOutputDTO

static/
 ├── app.js
 ├── main.css
 └── index.html
```

---

# 🔄 Funcionamento do WebSocket

## Endpoint de conexão

```http id="82dks1"
ws://localhost:8080/buildrun-livechat-websocket
```

## Fluxo de mensagens

1. Cliente conecta ao WebSocket
2. Cliente envia mensagem para:

```http id="2md91s"
/app/new-message
```

3. Servidor processa mensagem
4. Mensagem é publicada no tópico:

```http id="9d2ks1"
/topics/livechat
```

5. Todos os usuários conectados recebem a mensagem em tempo real

---

# 📡 Configuração STOMP

## Prefixos utilizados

### Aplicação

```bash id="92md8s"
/app
```

### Broker

```bash id="81dm2s"
/topics
```

---

# 📚 Conceitos aplicados

* WebSocket
* Comunicação em tempo real
* STOMP Protocol
* Publish/Subscribe
* SockJS
* DTO Pattern
* Event Driven
* Front-end integrado com Spring Boot
* Manipulação de DOM
* Segurança contra XSS

---

# ▶ Como executar

## Pré-requisitos

* Java 17+
* Maven

## Passos

1. Clone o repositório
2. Execute a aplicação Spring Boot
3. Acesse:

```bash id="92md1s"
http://localhost:8080
```

4. Informe um nome de usuário
5. Conecte ao chat
6. Envie mensagens em tempo real

---

# 🔥 Diferenciais do projeto

* Comunicação instantânea
* Arquitetura WebSocket completa
* Integração STOMP + SockJS
* Interface moderna
* Atualização em tempo real sem refresh
* Estrutura simples e escalável

---

# 👨‍💻 Autor

Felipe Movio

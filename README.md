# 🟢 Sistema de Gestão de Restaurantes — Serviços Node.js

Serviço auxiliar responsável por funcionalidades assíncronas e comunicação em tempo real, como **atualização de status e notificações**.

## 🛠️ Tecnologias

* Node.js
* Express
* WebSocket

## 🚀 Execução local

```bash
git clone <URL_DO_REPOSITORIO>
cd service
npm install
npm run dev
```

Configure o `.env` utilizando o `.env.example`.

## 🌿 Branches

A `main` contém apenas versões estáveis.

Para iniciar uma tarefa:

```bash
git checkout main
git pull origin main
git checkout -b feature/nome-da-tarefa
```

Exemplos:

```text
feature/websocket
feature/order-status
feature/notifications
fix/order-events
```

Tipos:

* `feature/` — nova funcionalidade
* `fix/` — correção
* `refactor/` — refatoração
* `docs/` — documentação

Ao finalizar:

```bash
git add .
git commit -m "feat: implement order status events"
git push origin feature/order-status
```

Abra um **Pull Request para `main`**.

## 📝 Commits

```text
tipo: descrição
```

Exemplo:

```text
feat: implement order status events
```

Tipos principais:

* `feat`
* `fix`
* `refactor`
* `test`
* `docs`
* `style`
* `build`
* `perf`

## 📂 Estrutura

```text
src/
├── routes/
├── controllers/
├── services/
├── websocket/
└── utils/
```

## ⚠️ Regras

* Não realizar `push` diretamente na `main`.
* Não versionar `.env`.
* Manter o serviço focado nas responsabilidades auxiliares.
* Testar alterações antes de abrir o PR.
* Documentar alterações que afetem a comunicação com os outros serviços.

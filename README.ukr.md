**Читати іншою мовою: [Українська](README.ukr.md), [English](README.md).**

# Chat app server

---

[![GraphQL](https://img.shields.io/badge/GraphQl-E10098?style=for-the-badge&logo=graphql&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](#)
[![ApolloGraphQL](https://img.shields.io/badge/-ApolloGraphQL-311C87?style=for-the-badge&logo=apollo-graphql)](#)
[![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)](#)
[![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)](#)
[![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)](#)

Це сервер Express/GraphQL/Apollo, створений та налаштований для додатку **Chat Application**

Це сервер Express/GraphQL із вбудованою невеликою базою даних SQLite. Він використовує JSON Web Token для автентифікації користувачів. Ще однією особливістю є підтримка протоколу WebSocket, який забезпечує двосторонній зв’язок між клієнтом і сервером через одне постійне TCP-з’єднання.

Цей сервер також використовує GraphQL Subscriptions, що разом із протоколом WebSocket дає нам можливість отримувати свіжі дані миттєво, без окремих запитів.

Як клієнт, так і сервер можуть надсилати повідомлення один одному одночасно, що робить це ідеальним для застосунків у реальному часі.

Цей сервер — лише частина додатку, друга частина (клієнтська) знаходиться в цьому репо: [Chat client](https://github.com/labattaria/chat-app-client)

Застосунок у цьому репозиторії розгорнуто за адресою: [https://render.com](https://render.com), за цією URL-адресою: [https://chat-app-server-0qdt.onrender.com/graphql](https://chat-app-server-0qdt.onrender.com/graphql)

Але ви можете використовувати цей сервер вручну на своєму локальному комп’ютері

## Залежностi, якi використовуються:

- **GraphQL** - Основна бібліотека GraphQL
- **Graphql-subscriptions** – Дозволяє реалізувати GraphQL-підписки для надсилання даних у реальному часі клієнтам
- **Graphql-ws** – Реалізація транспорту WebSocket для GraphQL-підписок
- **Apollo-server** - GraphQL-сервер, який працює з будь-якою схемою GraphQL
- **SQLite** - Легка, автономна SQL-база даних. Весь вміст зберігається в одному файлі
- **JWT (JSON Web Token)** - Компактний, безпечний для URL формат токена, який використовується для безпечної передачі інформації між сторонами. Зазвичай застосовується для автентифікації та авторизації у вебзастосунках
- **Nodemon** - Утиліта для розробки, яка автоматично перезапускає ваш сервер Node.js при виявленні змін у файлах

Повний список залежностей можна знайти у файлі **package.json**

---

## Вміст

- [Встановлення](#Встановлення)
- [Використання](#Використання)

### Встановлення

1. Склонуйте репозиторій:

```shell
git clone https://github.com/labattaria/chat-app-server.git
```

2. Встановіть залежності проекту:

```shell
cd chat-app-server
npm install
```

### Використання

Запустіть сервер за допомогою наступної команди:

```shell
npm start
```

Сервер буде доступний за адресою **http://localhost:9000/graphql**

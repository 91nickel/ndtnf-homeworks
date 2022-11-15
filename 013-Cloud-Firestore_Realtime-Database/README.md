# Домашнее задание к занятию «3.1 Cloud Firestore, Realtime Database»

**Правила выполнения домашней работы:**
* Выполняйте домашнее задание в отдельной ветке проекта на гитхабе.
* В поле для сдачи работы прикрепите ссылку на ваш проект в Git.
* Присылать на проверку можно каждую задачу по отдельности или все задачи вместе.
* Во время проверки по частям ваша домашняя работа будет со статусом «На доработке».
* Любые вопросы по решению задач задавайте в Slack.

**Задание 1**

Зарегистрируйте аккаунт [Firebase](https://firebase.google.com/) и создайте новый проект. 

**Задание 2**

Создайте новый проект NestJS.
> Можно взять за основу решение из домашнего задания [«2.3 Подключение базы данных к NestJS (модуль для MongoDB)»](https://github.com/netology-code/ndtnf-homeworks/tree/master/008-nestjs-db)  



Установите пакет [firebase-admin](https://firebase.google.com/docs/admin/setup#prerequisites) и проинициализируйте его, связав со своим приложением **Firebase**.

**Задание 3**

Ознакомьтесь с документацией  [Cloud Firestore](https://firebase.google.com/docs/firestore), [Realtime Database](https://firebase.google.com/docs/database) и выберите один из инструментов в качестве основного.

Перепишите приложение с использованием выбранного инструмента, реализовав описанную бизнес-логику.   

метод | url | действие | комментарий
--- | --- | ---  | ---
`GET` | `/api/books` | получить все книги | получаем массив всех книг
`GET` | `/api/books/:id` | получить книгу по **id** | получаем объект книги, если запись не найдено вернем **Code: 404** 
`POST` | `/api/books` | создать книгу | создаем кногу и возврашаем ее же вместе с присвоенным **id**
`PUT` | `/api/books/:id` | редактировать книгу по **id** |  редактируем объект книги, если запись не найдено вернем **Code: 404**
`DELETE` | `/api/books/:id` | удалить книгу по **id** | удаляем книгу и возвращаем ответ: **'ok'**


https://github.com/91nickel/netology-books/tree/firebase  
В main.ts - подключение бд https://github.com/91nickel/netology-books/blob/firebase/books_nest/src/main.ts  
Маршруты - https://github.com/91nickel/netology-books/blob/firebase/books_nest/src/books/books.controller.ts  
Сервис - https://github.com/91nickel/netology-books/blob/firebase/books_nest/src/books/books.service.ts  
  

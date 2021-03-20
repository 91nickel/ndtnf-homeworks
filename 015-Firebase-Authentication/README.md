# Домашнее задание к занятию «3.3 Firebase Authentication»

**Правила выполнения домашней работы:**
* Выполняйте домашнее задание в отдельной ветке проекта на гитхабе.
* В поле для сдачи работы прикрепите ссылку на ваш проект в Git.
* Присылать на проверку можно каждую задачу по отдельности или все задачи вместе.
* Во время проверки по частям ваша домашняя работа будет со статусом «На доработке».
* Любые вопросы по решению задач задавайте в Slack.

**Задание 1**

Ознакомитесь с документацией [Firebase Authentication](https://firebase.google.com/docs/auth)

**Задание 2**

Реализуйте роуты с использованием **admin.auth()**:

метод | url | действие 
--- | --- | --- 
`GET` | `/user/login` | страница с формой входа / регистрации
`GET` | `/user/profile` | страница профиля
`POST` | `/user/login` | авторизация пользователя
`POST` | `/user/signup` | регистрация пользователя  
`POST` | `/user/logout` | выход из системы

**не забудьте активировать необходимые **«Sign-in method»** в своем проекте Firebase*
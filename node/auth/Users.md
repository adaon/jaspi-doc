Users
================================================================================

Представляет коллекцию пользователей, хранящуюся в базе данных.

Расширяет `models.List`.

### init(url)
> Конструктор.

* **url**: URL-строка соединения с базой данных.

### register(props, callback)
> Регистрирует нового пользователя.

* **props**: Свойства создаваемого пользователя.
* **callback**: Функция обратного вызова. Получает массив номеров ошибок в первом аргументе и объект User или null во втором.

### getUser(username, password, callback)
> Получает пользователя.

* **username**, **password**: Имя пользователя и пароль.
* **callback**: Получает в первом аргументе объект User, если аутентификация прошла успешно. В противном случае получает null.
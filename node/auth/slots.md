slots
================================================================================

### auth.login(request, callback)
> Слот аутентификации.

* **request.dbURL**: Строка соединения с базой данных.
* **request.username**: Имя пользователя.
* **request.password**: Пароль.
* **callback**: Принимает объект пользователя или null и строковой ключ сессии.

### auth.logout(request, callback)
> Завершает текущую сессию.

* **request.dbURL**: Строка соединения с базой данных.
* **request.sessionKey**: Строковой ключ сессии.

### auth.auth(request, callback)
> Производит авторизацию.

* **request.dbURL**: Строка соединения с базой данных.
* **request.sessionKey**: Строковой ключ сессии.
* **callback**: Принимает объект пользователя или null.

### auth.register(request, callback)
> Производит регистрацию пользователя.

* **request.dbURL**: Строка соединения с базой данных.
* **request.data**: Содержит регистрационные данные (username, password, email и т.д.).
* **callback**: Принимает объект пользователя.
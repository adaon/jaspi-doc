# auth

Модуль, предоставляющий методы для аутентификации и авторизации.

### getSessionKey()
> Возвращает текущий ключ сессии или null.

### setSessionKey(sessionKey)
> Устанавливает текущий ключ сессии.

* **sessionKey**: Строковой ключ сессии.

### removeSessionKey()
> Удаляет текущий ключ сессии.

### login(username, password, callback)
> Производит аутентификацию и устанавливает текущий ключ сессии.

* **username**: Имя пользователя.
* **password**: Пароль.
* **callback**: Получает объект пользователя или null, если аутентификация завершилась неудачно.

### logout(callback)
> Закрывает текущую сессию.

### auth(callback)
> Производит авторизацию по текущему ключу сессии.

* **callback**: Получает объект пользователя или null.

### register(user, callback)
> Производит регистрацию нового пользователя.

* **user**: Объект пользователя, содержащий свойства username, password и др.
* **callback**: Получает массив номеров ошибок или пустой массив, если регистрация прошла успешно.
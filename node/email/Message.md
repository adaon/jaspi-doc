# Message

### init(options)
> Конструктор.
* **options.from**: От кого.
* **options.password**: Пароль для SMTP-сервера.
* **options.to**: Кому.
* **options.subject**: Тема.
* **options.content**: Содержимое.
* **options.host**: Сервер. Если не указан, используется тот же сервер, что и в `options.from`.
* **options.user**: Имя пользователя. Если не указано, используется то же, что и в `options.from`.

### send(to)
> Отправить письмо.
* **to**: Email-адрес получателя. Если не указан, используется адрес, указанный при создании объекта.
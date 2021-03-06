# project

### createApplication(options)
> Создает и возвращает приложение.

* **options.url**: URL приложения.
* **options.handler**: Функция-обработчик запроса (принимает request, response, callback), строковое содержимое ответа или путь к `.html` файлу.
* **options.slots**: Объект, отображающий имена слотов на функции-обработчики. Может иметь древовидную структуру, в таком случае именем слота становится путь к обработчику, разделенный точками.

### createProject(options)
> Создает и возвращает проект.

* **options.staticDir**: Путь к директории статических файлов.
* **options.dbURL**: Строка соединения с базой данных.
* **options.slots**: Отображающий имена слотов на функции-обработчики. Может иметь древовидную структуру, в таком случае именем слота становится путь к обработчику, разделенный точками.
* **options.middleware**: Массив функций-прослоек. Каждая функция принимает объект запроса и функцию обратного вызова.
* **options.apps**: Объект, отображающий URL-адреса приложений на объекты, передаваемые в функцию `createApplication()`.
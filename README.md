# О репозитории
Репозиторий разработан в качестве практического задания на курсе SkillFactory: PHPPRO
Профессия Fullstack веб-разработчик на JavaScript и PHP

…

## Используемые технологии
* HTML
* JavaScript

## Лицензия
* MIT

## Использование
Опубликованная версия доступна по адресу:
[nick-voskoboinikov.github.io/module16_homework](https://nick-voskoboinikov.github.io/module16_homework/)

## О содержимом / Ссылки на выполненные задания:
1. [task 1.html](./task 1.html) - Написать код, который будет преобразовывать XML в JS-объект и выводить его в консоль.
2. [task 2.html](./task 2.html) - Создать JS-объект, который при преобразовании в JSON будет возвращать в качестве результата такую же JSON-строку, как в образце. Получившуюся строку вывести в консоль.
3. [task 3.html](./task 3.html) - Написать скрипт, который при открытии страницы будет делать следующее:
Если пользователь зашел в первый раз, вывести окно prompt с сообщением: «Добро пожаловать! Назовите, пожалуйста, ваше имя».
После того, как пользователь введет имя, записать имя, дату и время визита в localStorage.
Если пользователь открывает страницу не впервые (это можно узнать по наличию соответствующих записей в localStorage), вывести в alert сообщение вида: «Добрый день, *имя пользователя*! Давно не виделись. В последний раз вы были у нас *дата последнего посещения*» и перезаписать дату последнего посещения.
Дату можно вывести в любом удобочитаемом формате (не Timestamp, должен четко читаться день, месяц, год и время — часы и минуты).
4. [task 4.html](./task 4.html) - Создать Promise, в котором c задержкой в три секунды сгенерировать случайное целое число от 1 до 100. Для создания задержки использовать setTimeout. Если сгенерированное число четное — Promise выполнится успешно (resolve), если нечетное — выполнится с ошибкой (reject). После разрешения Promise обработать результат его выполнения и вывести сообщение в консоль:
* «Завершено успешно. Сгенерированное число — number», если Promise завершился успешно. Вместо number подставить сгенерированное число
* «Завершено с ошибкой. Сгенерированное число — number», если Promise завершился с ошибкой. Вместо number подставить сгенерированное число

5. [task 5.html](./task 5.html) - Написать код приложения, интерфейс которого состоит из поля ввода и кнопки «Получить список задач». При нажатии на кнопку нужно отправить запрос с помощью fetch на URL https://jsonplaceholder.typicode.com/users/3/todos. Число 3 представляет собой id пользователя, вместо него нужно подставить число, введенное в поле. Если пользователь с таким id существует, вернется список задач для этого пользователя, каждая задача представлена объектом вида:
> {
>     "userId": 3,
>     "id": 43,
>     "title": "tempore ut sint quis recusandae",
>     "completed": true
> }
Где title — описание задачи, а completed — флаг, отображающий, выполнена задача или нет. Вывести данный список на страницу, оформив соответствующим образом: в виде списка (ul или ol), выполненные задачи должны быть написаны зачеркнутым текстом. Если пользователь с введенным id не существует, вывести сообщение:
«Пользователь с указанным id не найден».
6. [task 6.html](./task 6.html) - Написать код приложения, интерфейс которого состоит из двух input и кнопки. В input можно ввести любое число.
Заголовок первого input — «номер страницы».
Заголовок второго input — «лимит».
Заголовок кнопки — «запрос».
При клике на кнопку происходит следующее:
Если число в первом input не попадает в диапазон от 1 до 10 или не является числом — выводится ниже текст «Номер страницы вне диапазона от 1 до 10»;
Если число во втором input не попадает в диапазон от 1 до 10 или не является числом — выводится ниже текст «Лимит вне диапазона от 1 до 10»;
Если и первый, и второй input не в диапазонах или не являются числами — выводится ниже текст «Номер страницы и лимит вне диапазона от 1 до 10»;
Если числа попадают в диапазон от 1 до 10 — сделать запрос по URL https://picsum.photos/v2/list?page=1&limit=10, где GET-параметр page — это число из первого input, а GET-параметр limit — это введённое число второго input.
Пример: если пользователь ввёл 5 и 7, то запрос будет вида https://picsum.photos/v2/list?page=5&limit=7.
После получения данных вывести список картинок на экран.
Если пользователь перезагрузил страницу, то ему должны показываться картинки из последнего успешно выполненного запроса (использовать localStorage).

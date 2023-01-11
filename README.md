# О репозитории
Репозиторий разработан в качестве практического задания на курсе SkillFactory: PHPPRO
Профессия Fullstack веб-разработчик на JavaScript и PHP

---

## Используемые технологии
* HTML
* JavaScript

## Лицензия
* MIT

## Использование
Опубликованная версия доступна по адресу:
[nick-voskoboinikov.github.io/module16_homework](https://nick-voskoboinikov.github.io/module16_homework/)

## О содержимом / Ссылки на выполненные задания:

<ol>
  <li>
    <p><a href="/module16_homework/task%201.html">task 1.html</a> - Написать код, который будет преобразовывать XML в JS-объект и выводить его в консоль.</p>
  </li>
  <li>
    <p><a href="/module16_homework/task%202.html">task 2.html</a> - Создать JS-объект, который при преобразовании в JSON будет возвращать в качестве результата такую же JSON-строку, как в образце. Получившуюся строку вывести в консоль.</p>
  </li>
  <li>
    <p><a href="/module16_homework/task%203.html">task 3.html</a> - Написать скрипт, который при открытии страницы будет делать следующее:
Если пользователь зашел в первый раз, вывести окно prompt с сообщением: «Добро пожаловать! Назовите, пожалуйста, ваше имя».
После того, как пользователь введет имя, записать имя, дату и время визита в localStorage.
Если пользователь открывает страницу не впервые (это можно узнать по наличию соответствующих записей в localStorage), вывести в alert сообщение вида: «Добрый день, <em>имя пользователя</em>! Давно не виделись. В последний раз вы были у нас <em>дата последнего посещения</em>» и перезаписать дату последнего посещения.
Дату можно вывести в любом удобочитаемом формате (не Timestamp, должен четко читаться день, месяц, год и время — часы и минуты).</p>
  </li>
  <li><a href="/module16_homework/task%204.html">task 4.html</a> - Создать Promise, в котором c задержкой в три секунды сгенерировать случайное целое число от 1 до 100. Для создания задержки использовать setTimeout. Если сгенерированное число четное — Promise выполнится успешно (resolve), если нечетное — выполнится с ошибкой (reject). После разрешения Promise обработать результат его выполнения и вывести сообщение в консоль:
    <ul>
      <li>«Завершено успешно. Сгенерированное число — number», если Promise завершился успешно. Вместо number подставить сгенерированное число</li>
      <li>«Завершено с ошибкой. Сгенерированное число — number», если Promise завершился с ошибкой. Вместо number подставить сгенерированное число</li>
    </ul>
  </li>
  <li><a href="/module16_homework/task%205.html">task 5.html</a> - Написать код приложения, интерфейс которого состоит из поля ввода и кнопки «Получить список задач». При нажатии на кнопку нужно отправить запрос с помощью fetch на URL https://jsonplaceholder.typicode.com/users/3/todos. Число 3 представляет собой id пользователя, вместо него нужно подставить число, введенное в поле. Если пользователь с таким id существует, вернется список задач для этого пользователя, каждая задача представлена объектом вида:
    <blockquote>
      <p>{
    “userId”: 3,
    “id”: 43,
    “title”: “tempore ut sint quis recusandae”,
    “completed”: true
}</p>
    </blockquote>
  </li>

<p>Где title — описание задачи, а completed — флаг, отображающий, выполнена задача или нет. Вывести данный список на страницу, оформив соответствующим образом: в виде списка (ul или ol), выполненные задачи должны быть написаны зачеркнутым текстом. Если пользователь с введенным id не существует, вывести сообщение: «Пользователь с указанным id не найден».</p>

  <li><a href="/module16_homework/task%206.html">task 6.html</a> - Написать код приложения, интерфейс которого состоит из двух input и кнопки. В input можно ввести любое число.
    <ul>
      <li>Заголовок первого input — «номер страницы».</li>
      <li>Заголовок второго input — «лимит».</li>
      <li>Заголовок кнопки — «запрос».
При клике на кнопку происходит следующее:</li>
      <li>Если число в первом input не попадает в диапазон от 1 до 10 или не является числом — выводится ниже текст «Номер страницы вне диапазона от 1 до 10»;</li>
      <li>Если число во втором input не попадает в диапазон от 1 до 10 или не является числом — выводится ниже текст «Лимит вне диапазона от 1 до 10»;</li>
      <li>Если и первый, и второй input не в диапазонах или не являются числами — выводится ниже текст «Номер страницы и лимит вне диапазона от 1 до 10»;</li>
      <li>Если числа попадают в диапазон от 1 до 10 — сделать запрос по URL https://picsum.photos/v2/list?page=1&amp;limit=10, где GET-параметр page — это число из первого input, а GET-параметр limit — это введённое число второго input.
        <blockquote>
          <p>Пример: если пользователь ввёл 5 и 7, то запрос будет вида https://picsum.photos/v2/list?page=5&amp;limit=7.</p>
        </blockquote>
      </li>
    </ul>
<p>После получения данных вывести список картинок на экран.
Если пользователь перезагрузил страницу, то ему должны показываться картинки из последнего успешно выполненного запроса (использовать localStorage).</p>
  </li>
</ol>


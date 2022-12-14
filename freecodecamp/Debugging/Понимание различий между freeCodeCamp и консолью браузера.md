# Понимание различий между freeCodeCamp и консолью браузера
Вы могли заметить, что некоторые испытания freeCodeCamp включают собственную консоль. Эта консоль ведет себя немного иначе, чем консоль браузера.

Есть много методов, которые можно использовать `console`для вывода сообщений. `log`, `warn`, и `clear`назвать несколько. Консоль freeCodeCamp будет выводить только `log`сообщения, а консоль браузера — все сообщения. Когда вы вносите изменения в свой код, он автоматически запускается и показывает журналы. После этого консоль freeCodeCamp очищается при каждом запуске вашего кода.

Сначала откройте консоль браузера, чтобы увидеть журналы. Для этого вы можете щелкнуть правой кнопкой мыши панель навигации freeCodeCamp вверху и выбрать `inspect`большинство браузеров. Затем найдите `console`вкладку в открывшемся окне.

После этого используйте `console.log`для регистрации `output`переменной. Просмотрите две консоли, чтобы увидеть журнал. Наконец, используйте `console.clear`после вашего журнала, чтобы очистить консоль браузера. Посмотрите разницу в двух консолях.

### Before
```javascript
let output = "Get this to show once in the freeCodeCamp console and not at all in the browser console";
```
### Answers
```javascript
let output = "Get this to show once in the freeCodeCamp console and not at all in the browser console";

console.log(output);
console.clear();
```

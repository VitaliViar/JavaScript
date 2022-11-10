# Используйте typeof для проверки типа переменной
Вы можете использовать `typeof`для проверки структуры данных или типа переменной. Это полезно при отладке при работе с несколькими типами данных. Если вы думаете, что добавляете два числа, но одно из них на самом деле является строкой, результаты могут быть неожиданными. Ошибки типов могут скрываться в вычислениях или вызовах функций. Будьте особенно осторожны при доступе к внешним данным и работе с ними в форме объекта нотации объектов JavaScript (JSON).

Вот несколько примеров использования `typeof`:
```javascript
console.log(typeof "");
console.log(typeof 0);
console.log(typeof []);
console.log(typeof {});
```
По порядку консоль отобразит строки `string`, `number`, `objectи object`.

JavaScript распознает семь примитивных (неизменяемых) типов данных: `Boolean, Null, Undefined, Number, String, Symbol`(новое в ES6) и `BigInt`(новое в ES2020), а также один тип для изменяемых элементов: `Object.` Обратите внимание, что в JavaScript массивы технически являются типом объекта.
## Instructions
Добавьте два `console.log()`оператора для проверки `typeof`каждой из двух переменных `seven`и `three`в коде.
### Before
```javascript
let seven = 7;
let three = "3";
console.log(seven + three);
// Only change code below this line
```
### Answers
```javascript
let seven = 7;
let three = "3";
console.log(seven + three);
// Only change code below this line
console.log(typeof seven);
console.log(typeof three);
```

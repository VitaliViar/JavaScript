# Используйте параметр Rest с параметрами функции
Чтобы помочь нам создавать более гибкие функции, ES6 вводит _параметр `rest`_ для параметров функции. С помощью параметра `rest` вы можете создавать функции, которые принимают переменное количество аргументов. Эти аргументы хранятся в массиве, доступ к которому можно получить позже из функции.

Проверьте этот код:
```javascript
function howMany(...args) {
  return "You have passed " + args.length + " arguments.";
}
console.log(howMany(0, 1, 2));
console.log(howMany("string", null, [1, 2, 3], { }));
```
Консоль отобразит строки `You have passed 3 arguments.`и `You have passed 4 arguments.`.

Параметр `rest` избавляет от необходимости проверять `args`массив и позволяет применять `map()`, `filter()`и `reduce()`к массиву параметров.
## Instructions
Измените функцию, `sum`используя оставшийся параметр, таким образом, чтобы функция `sum`могла принимать любое количество аргументов и возвращать их сумму.
### Before
```javascript
const sum = (x, y, z) => {
  const args = [x, y, z];
  return args.reduce((a, b) => a + b, 0);
}
```
### Answers

```javascrit
const sum = (...args) => {
  return args.reduce((a, b) => a + b, 0);
}
```

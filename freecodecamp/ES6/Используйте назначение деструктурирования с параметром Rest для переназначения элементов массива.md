# Используйте назначение деструктурирования с параметром Rest для переназначения элементов массива
В некоторых ситуациях, связанных с деструктурированием массива, мы можем захотеть собрать остальные элементы в отдельный массив.

Результат аналогичен `Array.prototype.slice()`, как показано ниже:
```javascript
const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];
console.log(a, b);
console.log(arr);
```
Консоль отобразит значения `1`, `2`и `[3, 4, 5, 7]`.

Переменные aи bпринимают первое и второе значения из массива. После этого из-за наличия параметра `rest arr`получает остальные значения в виде массива. Остальной элемент корректно работает только как последняя переменная в списке. Например, вы не можете использовать параметр `rest` для захвата подмассива, в котором отсутствует последний элемент исходного массива.

Используйте присваивание деструктурирования с параметром `rest`, чтобы выполнить эффективный `Array.prototype.slice()`так, чтобы `arr`это был подмассив исходного массива `source`с опущенными первыми двумя элементами.
### Before
```javascript
const source = [1,2,3,4,5,6,7,8,9,10];
function removeFirstTwo(list) {
  // Only change code below this line
  const arr = list; // Change this line
  // Only change code above this line
  return arr;
}
const arr = removeFirstTwo(source);
```
### Answers
```javascript
const source = [1,2,3,4,5,6,7,8,9,10];
function removeFirstTwo(list) {
  // Only change code below this line
 const [a, b, ...arr] = list; // Change this line
  // Only change code above this line
  return arr;
}
const arr = removeFirstTwo(source);
```

# Добавить элементы с помощью splice()
Помните, в прошлой задаче мы упоминали, что `splice()`она может принимать до трех параметров? Что ж, вы можете использовать третий параметр, состоящий из одного или нескольких элементов, для добавления в массив. Это может быть невероятно полезно для быстрого переключения элемента или набора элементов на другой.
```javascript

const numbers = [10, 11, 12, 12, 15];
const startIndex = 3;
const amountToDelete = 1;

numbers.splice(startIndex, amountToDelete, 13, 14);
console.log(numbers);
```
Второе вхождение `12`удаляется, и мы добавляем `13`и `14`по тому же индексу. Теперь `numbers`массив будет `[ 10, 11, 12, 13, 14, 15 ]`.

Здесь мы начинаем с массива чисел. Затем мы передаем в `splice()`: индекс, с которого нужно начать удаление элементов `(3)`, количество удаляемых элементов `(1)` и оставшиеся аргументы `(13, 14)` будут вставлены, начиная с того же индекса. Обратите внимание, что после может быть любое количество элементов (разделенных запятыми) `amountToDelete`, каждый из которых будет вставлен.

Мы определили функцию `htmlColorNames`, которая принимает массив цветов HTML в качестве аргумента. Измените функцию, используя `splice()`для удаления первых двух элементов массива и добавления `'DarkSalmon'`и `'BlanchedAlmond'`в их соответствующих местах.
### Before
```javascript
function htmlColorNames(arr) {
  // Only change code below this line

  // Only change code above this line
  return arr;
}

console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurquoise', 'FireBrick']));
```
### Answers
```javascript
function htmlColorNames(arr) {
  // Only change code below this line
arr.splice(0, 2, 'DarkSalmon', 'BlanchedAlmond');
  // Only change code above this line
  return arr;
}

console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurquoise', 'FireBrick']));
```

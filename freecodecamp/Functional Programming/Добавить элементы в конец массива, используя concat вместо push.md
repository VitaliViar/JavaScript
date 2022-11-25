# Добавить элементы в конец массива, используя concat вместо push
Функциональное программирование — это создание и использование неизменяемых функций.

Последняя задача представила `concat`метод как способ объединения массивов в новый массив без изменения исходных массивов. Сравните `concat`с `push`методом. `push`добавляет элементы в конец того же массива, для которого он вызывается, что изменяет этот массив. Вот пример:
```javascript
const arr = [1, 2, 3];
arr.push(4, 5, 6);
```
`arr`будет иметь измененное значение `[1, 2, 3, 4, 5, 6]`, что не является способом функционального программирования.

`concat`предлагает способ объединения новых элементов в конец массива без каких-либо побочных эффектов мутации.

Измените `nonMutatingPush`функцию, чтобы она использовалась `concat`для слияния `newItem`до конца `original`без мутаций `original`или `newItem`массивов. Функция должна возвращать массив.

### Before
```javascript
function nonMutatingPush(original, newItem) {
  // Only change code below this line
  return original.push(newItem);

  // Only change code above this line
}

const first = [1, 2, 3];
const second = [4, 5];
nonMutatingPush(first, second);
```
### Answers
```javascript
function nonMutatingPush(original, newItem) {
  // Only change code below this line
  return original.concat(newItem);

  // Only change code above this line
}

const first = [1, 2, 3];
const second = [4, 5];
nonMutatingPush(first, second);
```

# Сортировка массива по алфавиту с помощью метода sort
Метод `sort`сортирует элементы массива в соответствии с функцией обратного вызова.

Например:
```javascript
function ascendingOrder(arr) {
  return arr.sort(function(a, b) {
    return a - b;
  });
}

ascendingOrder([1, 5, 2, 3, 4]);
Это вернет значение [1, 2, 3, 4, 5].

function reverseAlpha(arr) {
  return arr.sort(function(a, b) {
    return a === b ? 0 : a < b ? 1 : -1;
  });
}

reverseAlpha(['l', 'h', 'z', 'b', 's']);
```
Это вернет значение `['z', 's', 'l', 'h', 'b']`.

Метод сортировки по умолчанию в JavaScript — по строковому значению точки `Unicode`, что может привести к неожиданным результатам. Поэтому рекомендуется предоставлять функцию обратного вызова, чтобы указать, как сортировать элементы массива. Когда такая функция обратного вызова, обычно называемая `compareFunction`, предоставляется, элементы массива сортируются в соответствии с возвращаемым значением `compareFunction`: Если `compareFunction(a,b)`возвращает значение меньше `0` для двух элементов aи `b`, то aбудет стоять перед `b`. Если `compareFunction(a,b)`возвращает значение больше `0` для двух элементов `a`и `b`, то `b`будет стоять перед `a`. Если `compareFunction(a,b)`возвращает значение, равное `0` для двух элементов `a`и `b`, то `a`и `b`останется без изменений.

Используйте `sort`метод в `alphabeticalOrder`функции для сортировки элементов `arr`в алфавитном порядке. Функция должна возвращать отсортированный массив.

### Before
```javascript
function alphabeticalOrder(arr) {
  // Only change code below this line

  return arr
  // Only change code above this line
}

alphabeticalOrder(["a", "d", "c", "a", "z", "g"]);
```
### Answers
```javascript
function alphabeticalOrder(arr) {
  // Only change code below this line
  return arr.sort(function(a, b) {
    return a === b ? 0 : a < b ? -1 : 1;
  });
}

  // Only change code above this line

alphabeticalOrder(["a", "d", "c", "a", "z", "g"]);
```

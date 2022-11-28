Используйте метод some для проверки соответствия любых элементов массива критериям
Метод someработает с массивами, чтобы проверить, проходит ли какой -либо элемент определенный тест. Он возвращает логическое значение — trueесли какое-либо из значений соответствует критериям, falseесли нет.

Например, следующий код проверяет, numbersменьше ли какой-либо элемент в массиве 10:

const numbers = [10, 50, 8, 220, 110, 11];

numbers.some(function(currentValue) {
  return currentValue < 10;
});
Метод someвернет true.

Используйте someметод внутри checkPositiveфункции, чтобы проверить, является ли какой-либо элемент arrположительным. Функция должна возвращать логическое значение.
### Before
```javascript
function checkPositive(arr) {
  // Only change code below this line


  // Only change code above this line
}

checkPositive([1, 2, 3, -4, 5]);
```
### Answers
```javascript

```

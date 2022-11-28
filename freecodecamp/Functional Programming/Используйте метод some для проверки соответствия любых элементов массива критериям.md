# Используйте метод some для проверки соответствия любых элементов массива критериям
Метод `some`работает с массивами, чтобы проверить, проходит ли какой -либо элемент определенный тест. Он возвращает логическое значение — `true`если какое-либо из значений соответствует критериям, `false`если нет.

Например, следующий код проверяет, `numbers`меньше ли какой-либо элемент в массиве `10`:
```javascript
const numbers = [10, 50, 8, 220, 110, 11];

numbers.some(function(currentValue) {
  return currentValue < 10;
});
```
Метод `some`вернет `true`.

Используйте `some`метод внутри `checkPositive`функции, чтобы проверить, является ли какой-либо элемент arrположительным. Функция должна возвращать логическое значение.
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
function checkPositive(arr) {
  // Only change code below this line
return arr.some(val => val > 0);

  // Only change code above this line
}

checkPositive([1, 2, 3, -4, 5]);
```

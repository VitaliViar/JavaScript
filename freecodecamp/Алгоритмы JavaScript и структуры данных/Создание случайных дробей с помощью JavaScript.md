# Создание случайных дробей с помощью JavaScript
Случайные числа полезны для создания случайного поведения.

В JavaScript есть `Math.random()`функция, которая генерирует случайное десятичное число между `0`(включительно) и `1`(исключительно). Таким образом `Math.random()`, может вернуть a, `0`но никогда не вернуть a `1`.

### Примечание.
Как и [при сохранении значений с помощью оператора присваивания](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/storing-values-with-the-assignment-operator) , все вызовы функций будут разрешены до выполнения `return`, поэтому мы можем получить `return`значение `Math.random()`функции.

## Instructions

Измените `randomFraction`, чтобы возвращать случайное число вместо возврата `0`.
 ### Before
 
 ```javascript
 function randomFraction() {

  // Only change code below this line

  return 0;

  // Only change code above this line
}
 ```
 ### Answers
 
 ```javascript
 function randomFraction() {

  // Only change code below this line

  return Math.random (1);

  // Only change code above this line
}
 ```

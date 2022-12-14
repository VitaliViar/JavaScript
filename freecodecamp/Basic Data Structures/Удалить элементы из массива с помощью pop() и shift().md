# Удалить элементы из массива с помощью pop() и shift()

Оба `push()`и `unshift()`имеют соответствующие методы, которые почти функционально противоположны: `pop()`и `shift()`. Как вы уже, наверное, догадались, вместо добавления `pop()` удаляет элемент с конца массива, а `shift()`удаляет элемент с начала. Ключевое различие между `pop()`и `shift()`и их двоюродными братьями `push()`и `unshift()`, заключается в том, что ни один из методов не принимает параметры, и каждый из них позволяет изменять массив только одним элементом за раз.

Давайте взглянем:
```javascript
let greetings = ['whats up?', 'hello', 'see ya!'];

greetings.pop();
```
`greetings`будет иметь значение `['whats up?', 'hello']`.
```javascript
greetings.shift();
```
`greetings`будет иметь значение `['hello']`.

Мы также можем вернуть значение удаленного элемента любым из следующих методов:
```javascript
let popped = greetings.pop();
```
`greetings`будет иметь значение `[]`, и `popped`будет иметь значение `hello`.

Мы определили функцию `popShift`, которая принимает массив в качестве аргумента и возвращает новый массив. Измените функцию, используя `pop()`и `shift()`, чтобы удалить первый и последний элементы массива аргументов и присвоить удаленные элементы соответствующим переменным, чтобы возвращаемый массив содержал их значения.
### Before
```javascript
function popShift(arr) {
  let popped; // Change this line
  let shifted; // Change this line
  return [shifted, popped];
}

console.log(popShift(['challenge', 'is', 'not', 'complete']));
```
### Answers
```javascript
function popShift(arr) {
  let popped = arr.pop(); // Change this line
  let shifted = arr.shift(); // Change this line
  return [shifted, popped];
}

console.log(popShift(['challenge', 'is', 'not', 'complete']));
```

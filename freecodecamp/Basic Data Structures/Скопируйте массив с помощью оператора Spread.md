# Скопируйте массив с помощью оператора Spread
В то время как позволяет нам выбирать, какие элементы массива копировать, помимо нескольких других полезных задач, новый оператор распространения`slice()` ES6 позволяет нам легко копировать все элементы массива по порядку с помощью простого и легко читаемого синтаксиса. Синтаксис распространения выглядит следующим образом:...

На практике мы можем использовать оператор распространения для копирования массива следующим образом:
```javascript
let thisArray = [true, true, undefined, false, null];
let thatArray = [...thisArray];
```
`thatArray`равно `[true, true, undefined, false, null]. thisArray`остается неизменным и `thatArray`содержит те же элементы, что и `thisArray`.

Мы определили функцию, `copyMachine`которая принимает `arr(массив)` и `num(число)` в качестве аргументов. Предполагается, что функция возвращает новый массив, состоящий из `num`копий файлов `arr`. Мы сделали большую часть работы за вас, но она пока не работает должным образом. Измените функцию, используя синтаксис расширения, чтобы она работала правильно (подсказка: здесь может пригодиться другой метод, который мы уже рассмотрели!).



### Before
```javascript
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
    // Only change code below this line

    // Only change code above this line
    num--;
  }
  return newArr;
}

console.log(copyMachine([true, false, true], 2));

```
### Answers
```javascript
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
    // Only change code below this line
newArr.push([...arr]);
    // Only change code above this line
    num--;
  }
  return newArr;
}

console.log(copyMachine([true, false, true], 2));
```

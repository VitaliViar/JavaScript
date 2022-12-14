# Добавить элементы в массив с помощью push() и unshift()
Длина массива, как и типы данных, которые он может содержать, не фиксирована. Массивы могут быть определены с длиной любого количества элементов, и элементы могут добавляться или удаляться с течением времени; другими словами, массивы изменяемы . В этом задании мы рассмотрим два метода, с помощью которых мы можем программно изменить массив: `Array.push()и Array.unshift()`.

Оба метода принимают один или несколько элементов в качестве параметров и добавляют эти элементы в массив, для которого вызывается метод; метод `push()`добавляет элементы в конец массива и `unshift()`добавляет элементы в начало. Рассмотрим следующее:
```javascript
let twentyThree = 'XXIII';
let romanNumerals = ['XXI', 'XXII'];

romanNumerals.unshift('XIX', 'XX');
```
`romanNumerals`будет иметь значение `['XIX', 'XX', 'XXI', 'XXII']`.
```javascript
romanNumerals.push(twentyThree);
```
`romanNumerals`будет иметь значение `['XIX', 'XX', 'XXI', 'XXII', 'XXIII']`. Обратите внимание, что мы также можем передавать переменные, что дает нам еще большую гибкость при динамическом изменении данных нашего массива.

Мы определили функцию `mixedNumbers`, которой мы передаем массив в качестве аргумента. Измените функцию, используя `push()`и `unshift()`для добавления `'I', 2, 'three'`в начало массива и `7, 'VIII'`, `9`в конец, чтобы возвращаемый массив содержал представления чисел от `1` до `9` по порядку.

### Before
```javascript
function mixedNumbers(arr) {
  // Only change code below this line

  // Only change code above this line
  return arr;
}

console.log(mixedNumbers(['IV', 5, 'six']));
```
### Answers
```javascript
function mixedNumbers(arr) {
  // Only change code below this line
arr.unshift("I", 2, "three");
  arr.push(7, "VIII", 9);
  // Only change code above this line
  return arr;
}

console.log(mixedNumbers(['IV', 5, 'six']));
```

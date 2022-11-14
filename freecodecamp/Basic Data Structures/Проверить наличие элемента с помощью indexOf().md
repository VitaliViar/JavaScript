# Проверить наличие элемента с помощью indexOf()
Поскольку массивы могут быть изменены или _видоизменены_ в любое время, нет никакой гарантии относительно того, где конкретный фрагмент данных будет находиться в заданном массиве или существует ли этот элемент. К счастью, JavaScript предоставляет нам еще один встроенный метод, `indexOf()`который позволяет нам быстро и легко проверять наличие элемента в массиве. `indexOf()`принимает элемент в качестве параметра и при вызове возвращает позицию или индекс этого элемента, или `-1`если элемент не существует в массиве.

Например:
```javascript
let fruits = ['apples', 'pears', 'oranges', 'peaches', 'pears'];

fruits.indexOf('dates');
fruits.indexOf('oranges');
fruits.indexOf('pears');
```
`indexOf('dates')`возвращает `-1`, `indexOf('oranges')`возвращает `2`и `indexOf('pears')`возвращает `1`(первый индекс, по которому существует каждый элемент).

`indexOf()`может быть невероятно полезным для быстрой проверки наличия элемента в массиве. Мы определили функцию `quickCheck`, которая принимает массив и элемент в качестве аргументов. Измените функцию с помощью `indexOf()`так, чтобы она возвращала `true`значение, если переданный элемент существует в массиве, и `false`если его нет.


### Before
```javascript

function quickCheck(arr, elem) {
  // Only change code below this line

  // Only change code above this line
}

console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
```
### Answers
```javascript
function quickCheck(arr, elem) {
  // Only change code below this line
return arr.indexOf(elem) != -1;
  // Only change code above this line
}

console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
```

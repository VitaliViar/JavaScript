# Возвратите часть массива, используя метод slice
Метод sliceвозвращает копию определенных элементов массива. Он может принимать два аргумента, первый указывает индекс начала среза, второй — индекс конца среза (и он не является инклюзивным). Если аргументы не указаны, по умолчанию массив начинается с начала до конца, что является простым способом создания копии всего массива. Метод sliceне изменяет исходный массив, а возвращает новый.

Вот пример:

const arr = ["Cat", "Dog", "Tiger", "Zebra"];
const newArray = arr.slice(1, 3);
newArrayбудет иметь значение ["Dog", "Tiger"].

Используйте sliceметод в sliceArrayфункции, чтобы вернуть часть animмассива с учетом предоставленных beginSliceи endSliceиндексов. Функция должна возвращать массив.

### Before
```javascript
function sliceArray(anim, beginSlice, endSlice) {
  // Only change code below this line


  // Only change code above this line
}

const inputAnim = ["Cat", "Dog", "Tiger", "Zebra", "Ant"];
sliceArray(inputAnim, 1, 3);
```
### Answers
```javascript

```

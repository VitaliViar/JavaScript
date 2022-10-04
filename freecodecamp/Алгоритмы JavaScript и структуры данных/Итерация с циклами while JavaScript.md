# Итерация с циклами while JavaScript
Вы можете запустить один и тот же код несколько раз, используя цикл.

Первый тип цикла, который мы изучим, называется `while`циклом, потому что он выполняется, пока заданное условие истинно, и останавливается, когда это условие перестает быть истинным.

```javascript
const ourArray = [];
let i = 0;

while (i < 5) {
  ourArray.push(i);
  i++;
}
```
В приведенном выше примере кода `while`цикл выполнится 5 раз и добавит числа от 0 до 4 к `ourArray`.

Давайте попробуем заставить цикл `while` работать, помещая значения в массив.

## Instructions

Добавьте числа от 5 до 0 (включительно) в порядке убывания, чтобы `myArray`использовать `while`цикл.

### Before

```javascript
// Setup
const myArray = [];

// Only change code below this line
```
### Answers

```javascript
// Setup
const myArray = [5, 4, 3, 2, 1, 0];
let i = 5;

while (i < 0) {
  myArray.push(i);
  i++;
}
// Only change code below this line
```

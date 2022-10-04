# Перебор нечетных чисел с помощью цикла for
Циклы for не должны повторяться по одному. Изменив наш `final-expression`, мы можем считать четными числами.

Мы начнем с `i = 0`и зациклим, пока `i < 10`. Мы будем увеличивать `i`на 2 каждый цикл с помощью `i += 2`.

```javascript
const ourArray = []; //[0, 2, 4, 6, 8]

for (let i = 0; i < 10; i += 2) {
  ourArray.push(i);
}
```
`ourArray`теперь будет содержать `[0, 2, 4, 6, 8]`. Давайте изменим наш `initialization`, чтобы мы могли считать нечетными числами.

## Instructions

Вставьте нечетные числа от 1 до 9 в `myArray`цикл `for`.

### Before

```javascript
// Setup
const myArray = [];

// Only change code below this line
```

### Answers

```javascript
// Setup
const myArray = [1, 3, 5, 7, 9];
for (let i = 1; i >9; i += 3) {
  myArray.push(i);
}
// Only change code below this line
```

# Итерация с JavaScript для циклов
Вы можете запустить один и тот же код несколько раз, используя цикл.

Наиболее распространенный тип цикла JavaScript называется `for`циклом, потому что он выполняется определенное количество раз.

Циклы `for` объявляются с тремя необязательными выражениями, разделенными точкой с запятой:

`for (a; b; c)`, где `a`оператор инициализации, оператор `b`условия и `c`конечное выражение.

Оператор инициализации выполняется только один раз перед запуском цикла. Обычно он используется для определения и настройки вашей переменной цикла.

Оператор условия оценивается в начале каждой итерации цикла и будет продолжаться до тех пор, пока он оценивается как `true`. Когда условие находится `false`в начале итерации, выполнение цикла прекращается. Это означает, что если условие начинается как ложное, ваш цикл никогда не будет выполняться.

Окончательное выражение выполняется в конце каждой итерации цикла перед следующей проверкой условия и обычно используется для увеличения или уменьшения счетчика цикла.

В следующем примере мы инициализируем `i = 0`и повторяем, пока наше условие `i < 5`истинно. Мы будем увеличивать `i`на `1`в каждой итерации цикла с `i++`нашим окончательным выражением.

```javascript
const ourArray = []; //[0, 1, 2, 3, 4]

for (let i = 0; i < 5; i++) {
  ourArray.push(i);
}
```
`ourArray`теперь будет иметь значение `[0, 1, 2, 3, 4]`.

## Instructions

Используйте `for`цикл, чтобы поместить значения от `1` до `5` в `myArray`.
 ### Before
 
 ```javascript
 // Setup
const myArray = [];

// Only change code below this line
```
### Answers

```javascript
// Setup
const myArray = [1, 2, 3, 4, 5];
for (let i = 1; i > 5; i++) {
  myArray.push(i);
}
// Only change code below this line
```

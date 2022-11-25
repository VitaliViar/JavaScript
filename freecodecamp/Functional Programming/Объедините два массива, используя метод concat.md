# Объедините два массива, используя метод concat
Конкатенация означает соединение элементов встык. JavaScript предлагает `concat`метод как для строк, так и для массивов, которые работают одинаково. Для массивов метод вызывается для одного, затем в качестве аргумента передается другой массив concat, который добавляется в конец первого массива. Он возвращает новый массив и не изменяет ни один из исходных массивов. Вот пример:

[1, 2, 3].concat([4, 5, 6]);
Возвращаемый массив будет [1, 2, 3, 4, 5, 6].

Используйте concatметод в nonMutatingConcatфункции для конкатенации attachв конец original. Функция должна возвращать объединенный массив.
### Before
```javascript
function nonMutatingConcat(original, attach) {
  // Only change code below this line


  // Only change code above this line
}

const first = [1, 2, 3];
const second = [4, 5];
nonMutatingConcat(first, second);
```
### Answers
```javascript

```

# Объединение массивов с помощью оператора Spread
Еще одним огромным преимуществом оператора _расширения_ является возможность комбинировать массивы или вставлять все элементы одного массива в другой по любому индексу. С более традиционным синтаксисом мы можем объединять массивы, но это позволяет нам объединять массивы только в конце одного и в начале другого. Синтаксис расширения делает следующую операцию чрезвычайно простой:
```javascript
let thisArray = ['sage', 'rosemary', 'parsley', 'thyme'];

let thatArray = ['basil', 'cilantro', ...thisArray, 'coriander'];
```
`thatArray`будет иметь значение `['basil', 'cilantro', 'sage', 'rosemary', 'parsley', 'thyme', 'coriander']`.

Используя синтаксис расширения, мы только что выполнили операцию, которая была бы более сложной и многословной, если бы мы использовали традиционные методы.

Мы определили функцию `spreadOut`, которая возвращает переменную `sentence`. Измените функцию с помощью оператора распространения так, чтобы она возвращала массив `['learning', 'to', 'code', 'is', 'fun']`.

### Before
```javascript
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence; // Change this line
  return sentence;
}

console.log(spreadOut());

```
### Answers
```javascript
function spreadOut() {
  let fragment = ['to', 'code'];
  let setence = ["learning", ...fragment, "is", "fun"]; // Change this line
  return setence;
}

console.log(spreadOut());
```

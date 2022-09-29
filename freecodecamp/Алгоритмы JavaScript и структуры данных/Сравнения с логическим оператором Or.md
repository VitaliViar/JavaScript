# Сравнения с логическим оператором Or
Логический оператор _or_`||` ( ) возвращает trueзначение, если один из _операндов_ равен `true`. В противном случае возвращается `false`.

Логический оператор _or_ состоит из двух символов вертикальной черты: ( `||`). Обычно это можно найти между клавишами Backspace и Enter.

Шаблон ниже должен выглядеть знакомым по предыдущим путевым точкам:

```javascript

if (num > 10) {
  return "No";
}
if (num < 5) {
  return "No";
}
return "Yes";
```
вернется, `Yes`только если `num`находится между `5`и `10`(включая 5 и 10). Та же логика может быть записана как:

```javascript

if (num > 10 || num < 5) {
  return "No";
}
return "Yes";
```
## Instructions

Объедините два `if`оператора в один оператор, который возвращает строку `Outside`, если `val`она не находится между `10`и `20`включительно. В противном случае вернуть строку `Inside`.

### Before

```javascript

function testLogicalOr(val) {
  // Only change code below this line

  if (val) {
    return "Outside";
  }

  if (val) {
    return "Outside";
  }

  // Only change code above this line
  return "Inside";
}

testLogicalOr(15);
```
### Answers

```javascript
function testLogicalOr(val) {
  // Only change code below this line

  if (val < 10 || val > 20) {
    return "Outside";
  }
// Only change code above this line
  return "Inside";
}
testLogicalOr(15);
```

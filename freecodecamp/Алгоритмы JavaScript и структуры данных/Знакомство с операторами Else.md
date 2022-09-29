# Знакомство с операторами Else

Когда условие для `if`оператора истинно, выполняется блок кода, следующий за ним. Что делать, если это условие ложно? Обычно ничего бы не случилось. С `else`оператором может быть выполнен альтернативный блок кода.


```javascript

if (num > 10) {
  return "Bigger than 10";
} else {
  return "10 or Less";
}
```
## Instructions

Объедините `if`утверждения в одно `if/else`утверждение.

### Before

```javascript
function testElse(val) {
  let result = "";
  // Only change code below this line

  if (val > 5) {
    result = "Bigger than 5";
  }

  if (val <= 5) {
    result = "5 or Smaller";
  }

  // Only change code above this line
  return result;
}

testElse(4);
```
### Answers

```javascript

function testElse(val) {
  let result = "";
  // Only change code below this line

  if (val > 5) {
    return "Bigger than 5";
  } else {
return "5 or Smaller";

  //if (val <= 5) {
   // result = "5 or Smaller";
  }

  // Only change code above this line
  return result;
}

testElse(4);
```

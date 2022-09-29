# Знакомство с операторами Else If
Если у вас есть несколько условий, которые необходимо решить, вы можете связать `if`операторы вместе с `else if`операторами.

```javascript

if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}
```
## Instructions

Преобразуйте логику, чтобы использовать `else if`операторы.

### Before
```javascript

function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }

  if (val < 5) {
    return "Smaller than 5";
  }

  return "Between 5 and 10";
}

testElseIf(7);
```
### Answers

```javascript

function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }
else if (val < 5) {
    return "Smaller than 5";
  } else {
 return "Between 5 and 10";
}
}
testElseIf(7);
```

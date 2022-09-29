# Логический порядок в операторах If Else
Порядок важен в `if`, `else if`заявлениях.

Функция выполняется сверху вниз, поэтому вам нужно быть осторожным с тем, какой оператор идет первым.

Возьмите эти две функции в качестве примера.

### Вот первое:

```javascript

function foo(x) {
  if (x < 1) {
    return "Less than one";
  } else if (x < 2) {
    return "Less than two";
  } else {
    return "Greater than or equal to two";
  }
}
```
### А второй просто меняет порядок операторов:

```javascript

function bar(x) {
  if (x < 2) {
    return "Less than two";
  } else if (x < 1) {
    return "Less than one";
  } else {
    return "Greater than or equal to two";
  }
}
```
Хотя эти две функции выглядят почти одинаково, если мы передаем число обеим, мы получаем разные выходные данные.

```javascript

foo(0)
bar(0)
```
`foo(0)`вернет строку `Less than one`и `bar(0)`вернет строку `Less than two`.

## Instructions

Измените порядок логики в функции, чтобы она возвращала правильные операторы во всех случаях.

### Before

```javascript
 
 function orderMyLogic(val) {
  if (val < 10) {
    return "Less than 10";
  } else if (val < 5) {
    return "Less than 5";
  } else {
    return "Greater than or equal to 10";
  }
}

orderMyLogic(7);
```
### Answers

```javascript

function orderMyLogic(val) {
  if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}

orderMyLogic(7)
```

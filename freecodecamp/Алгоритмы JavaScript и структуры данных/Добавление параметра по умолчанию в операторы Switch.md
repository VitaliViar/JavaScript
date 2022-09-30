# Добавление параметра по умолчанию в операторы Switch
В `switch`операторе вы не сможете указать все возможные значения в качестве `case`операторов. Вместо этого вы можете добавить `default`оператор, который будет выполняться, если соответствующие `case`операторы не будут найдены. Думайте об этом как о последнем `else`утверждении в `if/else`цепочке.

Заявление `default`должно быть последним случаем.

```javascript

switch (num) {
  case value1:
    statement1;
    break;
  case value2:
    statement2;
    break;
...
  default:
    defaultStatement;
    break;
}
```
## Instructions

Напишите оператор `switch` для установки `answer`следующих условий:
* `a`- `apple`
* `b`- `bird`
* `c`- `cat`
* `default`-`stuff`

### Before

```javascript

function switchOfStuff(val) {
  let answer = "";
  // Only change code below this line



  // Only change code above this line
  return answer;
}

switchOfStuff(1);
```
### Answers

```javascript

function switchOfStuff(val) {
  let answer = "";
  // Only change code below this line

switch (val) {
  case "a":
    answer = "apple";
    break;
  case "b":
  answer = "bird";
    break;
  case "c":
 answer = "cat";
    break;
    case "d":
    answer = "stuff";
    break;
    case 4 :
    answer = "stuff";
    break;
    default:
    answer = "stuff";
    break;
}


  // Only change code above this line
  return answer;
}

switchOfStuff(1);
```

# Выбор из множества вариантов с операторами Switch
Если у вас есть много вариантов на выбор, используйте оператор _switch_ . Оператор `switch`проверяет значение и может иметь множество операторов _case_ , определяющих различные возможные значения. Операторы выполняются с первого совпавшего `case`значения до тех пор, пока `break`не встретится a.

### Вот пример `switch`заявления:

```javascript

switch (lowercaseLetter) {
  case "a":
    console.log("A");
    break;
  case "b":
    console.log("B");
    break;
}
```
`case`значения проверяются на строгое равенство (` ===`). Сообщает `break`JavaScript прекратить выполнение инструкций. Если `break`опущено, будет выполнен следующий оператор.

## Instructions

Напишите оператор `switch`, который проверяет `val`и устанавливает `answer`следующие условия:
* `1`- `alpha`
* `2`- `beta`
* `3`- `gamma`
* `4`-`delta`

### Before

```javascript

function caseInSwitch(val) {
  let answer = "";
  // Only change code below this line



  // Only change code above this line
  return answer;
}

caseInSwitch(1);
```
### Answers

```javascript

function caseInSwitch(val) {
  let answer = "";
  // Only change code below this line
switch (val) {
  case 1 :
  answer = "alpha";
  console.log("alpha");
  break;
  case 2 :
  answer = "beta";
  console.log("beta");
  break;
  case 3 :
  answer = "gamma";
  console.log("gamma");
  break;
  case 4 :
  answer = "delta";
  console.log("delta");
  break;
}


  // Only change code above this line
  return answer;
}

caseInSwitch(1);
```



# Несколько идентичных опций в операторах switch
Если `break`оператор отсутствует в `switch`операторе `case`, следующие `case`операторы выполняются до тех пор, пока `break`не встретится a. Если у вас есть несколько входов с одним и тем же выходом, вы можете представить их в таком `switch`выражении:

```javascript

let result = "";
switch (val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4 alone";
}
```
Варианты 1, 2 и 3 дадут одинаковый результат.

## Instructions

Напишите оператор `switch` для установки `answer`следующих диапазонов:
* `1-3`- `Low`
* `4-6`- `Mid`
* `7-9`-`High`

**Примечание.** Вам потребуется `case`заявление для каждого числа в диапазоне.

### Before

```javascript

function sequentialSizes(val) {
  let answer = "";
  // Only change code below this line



  // Only change code above this line
  return answer;
}

sequentialSizes(1);
```
### Answers

```javascript

function sequentialSizes(val) {
  let answer = "";
  // Only change code below this line
let result = "";
switch (val) {
  case 1:
  answer = "Low";
  return "Low";
  case 2:
  answer = "Low";
  return "Low";
  case 3:
  answer = "Low";
  return "Low";
  case 4:
  answer = "Mid";
  return "Mid";
  case 5:
  answer = "Mid";
  return "Mid";
  case 6:
  answer = "Mid";
  return "Mid";
  case 7:
  answer = "High";
  case 8:
  answer = "High";
  case 9:
  answer = "High";
}


  // Only change code above this line
  return answer;
}

sequentialSizes(1);
```

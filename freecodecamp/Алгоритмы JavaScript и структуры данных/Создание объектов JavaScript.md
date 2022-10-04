# Создание объектов JavaScript
Возможно, вы уже слышали этот термин `object`.

Объекты аналогичны `arrays`, за исключением того, что вместо использования индексов для доступа и изменения их данных вы получаете доступ к данным в объектах через то, что называется `properties`.

Объекты полезны для структурированного хранения данных и могут представлять объекты реального мира, например кошку.

### Вот пример объекта кошки:

```javascript
 
const cat = {
  "name": "Whiskers",
  "legs": 4,
  "tails": 1,
  "enemies": ["Water", "Dogs"]
};
```
В этом примере все свойства хранятся в виде строк, таких как `name`, `legs`и `tails`. Однако вы также можете использовать числа в качестве свойств. Вы даже можете опустить кавычки для строковых свойств, состоящих из одного слова, как показано ниже:

```javascript

const anotherObject = {
  make: "Ford",
  5: "five",
  "model": "focus"
};
```

Однако, если у вашего объекта есть какие-либо нестроковые свойства, JavaScript автоматически приведёт их к типу строк.

## Instructions

Создайте объект, представляющий вызываемую собаку, `myDog`который содержит свойства `name`(строку) `legs`, `tails`и `friends`.

Вы можете установить для этих свойств объекта любые значения, которые вы хотите, если `name`это строка, числа и `legs`массив .`tailsfriends`

### Before

```javascript

const myDog = {
  // Only change code below this line


  // Only change code above this line
};
```
### Answers

```javascript
const myDog = {
  // Only change code below this line
"name": "Daffna",
"legs": 4,
"tails": 1,
"friends": ["Vitali", "Nina"]

  // Only change code above this line
};
```


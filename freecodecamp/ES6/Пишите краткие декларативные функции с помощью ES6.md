# Пишите краткие декларативные функции с помощью ES6
При определении функций внутри объектов в ES5 мы должны использовать ключевое слово `function`следующим образом:
```javascript
const person = {
  name: "Taylor",
  sayHello: function() {
    return `Hello! My name is ${this.name}.`;
  }
}
```
В ES6 вы можете `function`полностью удалить ключевое слово и двоеточие при определении функций в объектах. Вот пример такого синтаксиса:
```javascript
const person = {
  name: "Taylor",
  sayHello() {
    return `Hello! My name is ${this.name}.`;
  }
};
```
Рефакторинг функции `setGear`внутри объекта `bicycle`для использования сокращенного синтаксиса, описанного выше.
### Before
```javascript
// Only change code below this line
const bicycle = {
  gear: 2,
  setGear: function(newGear) {
    this.gear = newGear;
  }
};
// Only change code above this line
bicycle.setGear(3);
console.log(bicycle.gear);
```
### Answers
```javascript
// Only change code below this line
const bicycle = {
  gear: 2,
  setGear (newGear) {
    this.gear = newGear;
  }
};
// Only change code above this line
bicycle.setGear(3);
console.log(bicycle.gear);
```

# Удалить свойства из объекта JavaScript
Мы также можем удалить свойства из объектов следующим образом:

```javascript

delete ourDog.bark;
```
### Пример:

```javascript

const ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};

delete ourDog.bark;
```
После последней строки, показанной выше, `ourDog`выглядит так:

```javascript

{
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
}
```

## Instructions

Удалить `tails`свойство из `myDog`. Вы можете использовать либо точку, либо квадратную нотацию.

### Before

```javascript

// Setup
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line
```

### Answers

```javascript

// Setup
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line
delete myDog.tails;
```

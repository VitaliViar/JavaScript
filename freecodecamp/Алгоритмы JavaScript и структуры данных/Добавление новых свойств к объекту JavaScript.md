# Добавление новых свойств к объекту JavaScript
Вы можете добавлять новые свойства к существующим объектам JavaScript так же, как вы их изменяете.

Вот как мы добавим `bark`свойство в `ourDog`:

```javascript

ourDog.bark = "bow-wow";
```
или же

```javascript 

ourDog["bark"] = "bow-wow";
```
Теперь, когда мы оценим `ourDog.bark`, мы получим его лай `bow-wow`.

### Пример:

```javascript 

const ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};
ourDog.bark = "bow-wow";
```

## Instructions

Добавьте `bark`свойство `myDog`и задайте для него звук собаки, например `"гав"`. Вы можете использовать либо точку, либо квадратную нотацию.

### Before

```javascript

const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
```
### Answers

```javascript

const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.bark = "bow-wow";
```


# Проверка конструктора объекта с помощью instanceof
Каждый раз, когда функция-конструктор создает новый объект, говорят, что этот объект является экземпляром своего конструктора. JavaScript дает удобный способ проверить это с `instanceof`оператором. `instanceof`позволяет сравнивать объект с конструктором, возвращая `true`или `false`основываясь на том, был ли этот объект создан с помощью конструктора. Вот пример:
```javascript
let Bird = function(name, color) {
  this.name = name;
  this.color = color;
  this.numLegs = 2;
}

let crow = new Bird("Alexis", "black");

crow instanceof Bird;
```
Этот `instanceof`метод вернет `true`.

Если объект создан без использования конструктора, `instanceof`будет проверено, что он не является экземпляром этого конструктора:
```javascript
let canary = {
  name: "Mildred",
  color: "Yellow",
  numLegs: 2
};

canary instanceof Bird;
```
Этот `instanceof`метод вернет `false`.

Создайте новый экземпляр `House`конструктора, вызвав его `myHouse`и передав количество спален. Затем используйте `instanceof`для проверки того, что это экземпляр `House`.

### Before
```javascript
function House(numBedrooms) {
  this.numBedrooms = numBedrooms;
}

// Only change code below this line
```
### Answers
```javascript
function House(numBedrooms) {
  this.numBedrooms = numBedrooms;
}

// Only change code below this line
let myHouse = new House(2);
myHouse instanceof House;
```

# Используйте Mixin для добавления общего поведения между несвязанными объектами
Как вы видели, поведение передается через наследование. Однако бывают случаи, когда наследование — не лучшее решение. Наследование плохо работает для несвязанных объектов, таких как `Bird`и `Airplane`. Они оба могут летать, но `Bird`не являются типом `Airplane`и наоборот.

Для несвязанных объектов лучше использовать миксины . `Mixin` позволяет другим объектам использовать набор функций.
```javascript
let flyMixin = function(obj) {
  obj.fly = function() {
    console.log("Flying, wooosh!");
  }
};
```
Берет `flyMixin`любой объект и дает ему `fly`метод.
```javascript
let bird = {
  name: "Donald",
  numLegs: 2
};

let plane = {
  model: "777",
  numPassengers: 524
};

flyMixin(bird);
flyMixin(plane);
```
Здесь `bird`и `plane`передаются в `flyMixin`, который затем присваивает `fly`функцию каждому объекту. Теперь `bird`и `plane`оба могут летать:
```javascript
bird.fly();
plane.fly();
```
Консоль будет отображать строку `Flying`, `wooosh`!дважды, по одному разу для каждого .`fly()`вызова.

Обратите внимание, как миксин позволяет `fly`повторно использовать один и тот же метод несвязанными объектами `bird`и файлами `plane`.

Создайте миксин с именем `glideMixin`, который определяет метод с именем `glide`. Затем используйте, `glideMixin`чтобы дать обоим `bird`и `boat`способность скользить.

### Before
```javascript
let bird = {
  name: "Donald",
  numLegs: 2
};

let boat = {
  name: "Warrior",
  type: "race-boat"
};

// Only change code below this line
```
### Answers
```javascript
let bird = {
  name: "Donald",
  numLegs: 2
};

let boat = {
  name: "Warrior",
  type: "race-boat"
};

// Only change code below this line
let glideMixin = function(obj) {
  obj.glide = function() {
    console.log("Gliding!");
  };
};
glideMixin(bird);
glideMixin(boat);
```

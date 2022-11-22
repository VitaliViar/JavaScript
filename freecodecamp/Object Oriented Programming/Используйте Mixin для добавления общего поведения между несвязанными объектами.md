Используйте Mixin для добавления общего поведения между несвязанными объектами
Как вы видели, поведение передается через наследование. Однако бывают случаи, когда наследование — не лучшее решение. Наследование плохо работает для несвязанных объектов, таких как Birdи Airplane. Они оба могут летать, но Birdне являются типом Airplaneи наоборот.

Для несвязанных объектов лучше использовать миксины . Mixin позволяет другим объектам использовать набор функций.

let flyMixin = function(obj) {
  obj.fly = function() {
    console.log("Flying, wooosh!");
  }
};
Берет flyMixinлюбой объект и дает ему flyметод.

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
Здесь birdи planeпередаются в flyMixin, который затем присваивает flyфункцию каждому объекту. Теперь birdи planeоба могут летать:

bird.fly();
plane.fly();
Консоль будет отображать строку Flying, wooosh!дважды, по одному разу для каждого .fly()вызова.

Обратите внимание, как миксин позволяет flyповторно использовать один и тот же метод несвязанными объектами birdи файлами plane.

Создайте миксин с именем glideMixin, который определяет метод с именем glide. Затем используйте, glideMixinчтобы дать обоим birdи boatспособность скользить.

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

```

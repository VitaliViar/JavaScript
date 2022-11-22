# Используйте IIFE для создания модуля
Немедленно вызываемое функциональное выражение (IIFE) часто используется для группировки связанных функций в один объект или _модуль_ . Например, более ранняя задача определила два миксина:
```javascript
function glideMixin(obj) {
  obj.glide = function() {
    console.log("Gliding on the water");
  };
}
function flyMixin(obj) {
  obj.fly = function() {
    console.log("Flying, wooosh!");
  };
}
```
Мы можем сгруппировать эти миксины в модуль следующим образом:
```javascript
let motionModule = (function () {
  return {
    glideMixin: function(obj) {
      obj.glide = function() {
        console.log("Gliding on the water");
      };
    },
    flyMixin: function(obj) {
      obj.fly = function() {
        console.log("Flying, wooosh!");
      };
    }
  }
})();
```
Обратите внимание, что у вас есть немедленно вызываемое функциональное выражение (IIFE), которое возвращает объект `motionModule`. Этот возвращенный объект содержит все варианты поведения примесей как свойства объекта. Преимущество модульного шаблона заключается в том, что все поведения движения могут быть упакованы в один объект, который затем может использоваться другими частями вашего кода. Вот пример его использования:
```javascript
motionModule.glideMixin(duck);
duck.glide();
```
Создайте модуль с именем `funModule`, чтобы обернуть два миксина `isCuteMixinи singMixin. funModule`должен вернуть объект.

### Before
```javascript
let isCuteMixin = function(obj) {
  obj.isCute = function() {
    return true;
  };
};
let singMixin = function(obj) {
  obj.sing = function() {
    console.log("Singing to an awesome tune");
  };
};
```
### Answers
```javascript
/*let isCuteMixin = function(obj) {
  obj.isCute = function() {
    return true;
  };
};
let singMixin = function(obj) {
  obj.sing = function() {
    console.log("Singing to an awesome tune");
  };
};
*/

let funModule = (function() {
  return {
    isCuteMixin: function(obj) {
      obj.isCute = function() {
        return true;
      };
    },
    singMixin: function(obj) {
      obj.sing = function() {
        console.log("Singing to an awesome tune");
      };
    }
  };
})();
```

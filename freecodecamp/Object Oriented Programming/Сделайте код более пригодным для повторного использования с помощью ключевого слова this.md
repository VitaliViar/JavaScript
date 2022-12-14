# Сделайте код более пригодным для повторного использования с помощью ключевого слова this
Последняя задача представила метод `duck`объекту. Он использовал` duck.name`точечную нотацию для доступа к значению `name`свойства в операторе `return:`
```javascript
sayName: function() {return "The name of this duck is " + duck.name + ".";}
```
Хотя это допустимый способ доступа к свойству объекта, здесь есть ловушка. Если имя переменной изменится, любой код, ссылающийся на исходное имя, также необходимо будет обновить. В коротком определении объекта это не проблема, но если объект имеет много ссылок на свои свойства, вероятность ошибки возрастает.

Чтобы избежать этих проблем, используйте `this`ключевое слово:
```javascript
let duck = {
  name: "Aflac",
  numLegs: 2,
  sayName: function() {return "The name of this duck is " + this.name + ".";}
};
```
`this`— глубокая тема, и приведенный выше пример — только один из способов ее использования. В текущем контексте `this`относится к объекту, с которым связан метод: `duck`. Если имя объекта изменено на `mallard`, нет необходимости искать `duck`в коде все ссылки на . Это делает код повторно используемым и более легким для чтения.

Измените `dog.sayLegs`метод, чтобы удалить любые ссылки на файлы `dog`. Используйте `duck`пример для руководства.

### Before
```javascript
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs: function() {return "This dog has " + dog.numLegs + " legs.";}
};

dog.sayLegs();
```
### Answers
```javascript
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs: function() {return "This dog has " + this.numLegs + " legs.";}
};

dog.sayLegs();
```

# Добавьте пары ключ-значение в объекты JavaScript
По своей сути объекты — это просто наборы пар ключ-значение . Другими словами, это фрагменты данных ( значения ), сопоставленные с уникальными идентификаторами, называемыми свойствами ( ключами ). Взгляните на пример:
```javascript
const tekkenCharacter = {
  player: 'Hwoarang',
  fightingStyle: 'Tae Kwon Doe',
  human: true
};
```
Приведенный выше код определяет объект персонажа видеоигры `Tekken` с именем `tekkenCharacter`. Он имеет три свойства, каждое из которых соответствует определенному значению. Если вы хотите добавить дополнительное свойство, например «происхождение», это можно сделать, присвоив `origin`объекту:
```javascript
tekkenCharacter.origin = 'South Korea';
```
При этом используется точечная запись. Если бы вы наблюдали за `tekkenCharacter`объектом, теперь он включал бы это `origin`свойство. У Хвоаранг также были отчетливые оранжевые волосы. Вы можете добавить это свойство с нотацией скобок, выполнив:
```javascript
tekkenCharacter['hair color'] = 'dyed orange';
```
Обозначение в квадратных скобках требуется, если в вашем свойстве есть пробел или если вы хотите использовать переменную для имени свойства. В приведенном выше случае свойство заключено в кавычки, чтобы обозначить его как строку, и будет добавлено точно так, как показано. Без кавычек оно будет оцениваться как переменная, и имя свойства будет любым значением переменной. Вот пример с переменной:
```javascript
const eyes = 'eye color';

tekkenCharacter[eyes] = 'brown';
```
После добавления всех примеров объект будет выглядеть так:
```javascript
{
  player: 'Hwoarang',
  fightingStyle: 'Tae Kwon Doe',
  human: true,
  origin: 'South Korea',
  'hair color': 'dyed orange',
  'eye color': 'brown'
};
```
Создан `foods`объект с тремя записями. Используя выбранный вами синтаксис, добавьте к нему еще три записи: `bananasсо` значением `13`, `grapes`со значением `35`и `strawberries`со значением `27`.

### Before
```javascript
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28
};

// Only change code below this line

// Only change code above this line

console.log(foods);
```
### Answers
```javascript
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28
};

// Only change code below this line
foods["bananas"] = 13;
  foods["grapes"] = 35;
  foods["strawberries"] = 27
// Only change code above this line

console.log(foods);
```


# Используйте ключевое слово delete для удаления свойств объекта
Теперь вы знаете, что такое объекты, их основные особенности и преимущества. Короче говоря, это хранилища ключей и значений, которые обеспечивают гибкий и интуитивно понятный способ структурирования данных и обеспечивают очень быстрое время поиска. В оставшейся части этих задач мы опишем несколько общих операций, которые вы можете выполнять с объектами, чтобы вам было удобно применять эти полезные структуры данных в своих программах.

В более ранних задачах мы как добавляли, так и изменяли пары ключ-значение объекта. Здесь мы увидим, как мы можем удалить пару ключ-значение из объекта.

Давайте еще foodsраз вернемся к нашему объектному примеру. Если мы хотим удалить applesключ, мы можем удалить его, используя deleteключевое слово, подобное этому:
```javascript
delete foods.apples;
```
## Instructions
Используйте ключевое слово `delete`, чтобы удалить ключи `oranges`, `plums`, и `strawberries`из `foods`объекта.

### Before
```javascript
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
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
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};

// Only change code below this line
delete foods.oranges; delete foods.plums; delete foods.strawberries;
// Only change code above this line

console.log(foods);
```

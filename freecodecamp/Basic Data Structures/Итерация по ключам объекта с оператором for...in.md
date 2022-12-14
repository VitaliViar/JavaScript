# Итерация по ключам объекта с оператором for...in
Иногда вам может понадобиться перебрать все ключи внутри объекта. Для этого требуется специальный синтаксис в JavaScript, называемый оператором `for...in` . Для нашего `users`объекта это может выглядеть так:
```javascript
for (let user in users) {
  console.log(user);
}
```
Это будет регистрировать `Alan`, `Jeff`и `Sarah`- каждое значение в отдельной строке.

В этом операторе мы определили переменную `user`, и, как вы можете видеть, эта переменная сбрасывалась во время каждой итерации для каждого из ключей объекта по мере того, как оператор проходил через объект, в результате чего имя каждого пользователя выводилось на консоль.

**ПРИМЕЧАНИЕ.** Объекты не сохраняют порядок хранимых ключей, как это делают массивы; таким образом, положение ключа на объекте или относительный порядок, в котором он появляется, не имеет значения при обращении к этому ключу или доступе к нему.

Мы определили функцию, `countOnline`которая принимает один аргумент (объект пользователя). Используйте оператор `for...in` в этой функции, чтобы пройти по объекту пользователей, переданному в функцию, и вернуть количество пользователей, чье `online`свойство установлено на `true`. Пример объекта пользователей, которому можно передать `countOnline`, показан ниже. У каждого пользователя будет `online`свойство со значением `true`или `false`.
```javascript
{
  Alan: {
    online: false
  },
  Jeff: {
    online: true
  },
  Sarah: {
    online: false
  }
}
```
### Before
```javascript
const users = {
  Alan: {
    online: false
  },
  Jeff: {
    online: true
  },
  Sarah: {
    online: false
  }
}

function countOnline(usersObj) {
  // Only change code below this line

  // Only change code above this line
}

console.log(countOnline(users));
```
### Answers
```javascript
const users = {
  Alan: {
    online: false
  },
  Jeff: {
    online: true
  },
  Sarah: {
    online: false
  }
}

function countOnline(usersObj) {
  // Only change code below this line
let result = 0;
  for (let user in usersObj) {
    if (usersObj[user].online === true) {
      result++;
    }
  }
  return result;
  // Only change code above this line
}

console.log(countOnline(users));
```



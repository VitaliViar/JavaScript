Добавить элементы в конец массива, используя concat вместо push
Функциональное программирование — это создание и использование неизменяемых функций.

Последняя задача представила concatметод как способ объединения массивов в новый массив без изменения исходных массивов. Сравните concatс pushметодом. pushдобавляет элементы в конец того же массива, для которого он вызывается, что изменяет этот массив. Вот пример:

const arr = [1, 2, 3];
arr.push(4, 5, 6);
arrбудет иметь измененное значение [1, 2, 3, 4, 5, 6], что не является способом функционального программирования.

concatпредлагает способ объединения новых элементов в конец массива без каких-либо побочных эффектов мутации.

Измените nonMutatingPushфункцию, чтобы она использовалась concatдля слияния newItemдо конца originalбез мутаций originalили newItemмассивов. Функция должна возвращать массив.

### Before
```javascript
function nonMutatingPush(original, newItem) {
  // Only change code below this line
  return original.push(newItem);

  // Only change code above this line
}

const first = [1, 2, 3];
const second = [4, 5];
nonMutatingPush(first, second);
```
### Answers
```javascript

```

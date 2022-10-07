# Используйте функцию parseInt с основанием
Функция `parseInt()`анализирует строку и возвращает целое число. Он принимает второй аргумент для системы счисления, который указывает основание числа в строке. Основание может быть целым числом от `2` до `36`.

Вызов функции выглядит так:
```javscript
parseInt(string, radix);
```
И вот пример:
```javascript
const a = parseInt("11", 2);
```
Переменная системы счисления говорит, что `11`она находится в двоичной системе или с основанием `2`. В этом примере строка преобразуется `11`в целое число `3`.

## Instuctions

Используйте `parseInt()`в `convertToInteger`функции, чтобы она преобразовывала двоичное число в целое и возвращала его.

### Before
```javascript
function convertToInteger(str) {

}

convertToInteger("10011");
```

### Answers
```javascript
function convertToInteger(str) {
return parseInt(str, 2);
}
convertToInteger("10011");
```


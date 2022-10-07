# Используйте функцию parseInt
Функция `parseInt()`анализирует строку и возвращает целое число. 
### Вот пример:
```javascript
const a = parseInt("007");
```
Приведенная выше функция преобразует строку `007`в целое число `7`. Если первый символ в строке не может быть преобразован в число, возвращается `NaN`.
## Instructions
Используйте `parseInt()`в `convertToInteger`функции, чтобы она преобразовывала входную строку `str`в целое число и возвращала ее.
### Before
```javascript
function convertToInteger(str) {

}
convertToInteger("56");
```
## Answers
```javascript
function convertToInteger(str) {
return parseInt(str);
}

convertToInteger("56");
```


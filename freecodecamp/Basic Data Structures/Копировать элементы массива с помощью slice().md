# Копировать элементы массива с помощью slice()
Следующий метод, который мы рассмотрим, это `slice()`. Вместо изменения массива `slice()`копирует или извлекает заданное количество элементов в новый массив, оставляя массив, к которому он вызывается, нетронутым. slice()принимает только 2 параметра — первый — это индекс, с которого следует начать извлечение, а второй — индекс, с которого следует остановить извлечение (извлечение будет происходить до, но не включая элемент с этим индексом). Учти это:

let weatherConditions = ['rain', 'snow', 'sleet', 'hail', 'clear'];

let todaysWeather = weatherConditions.slice(1, 3);
todaysWeatherбудет иметь значение ['snow', 'sleet'], в то время как weatherConditionsвсе еще будет иметь ['rain', 'snow', 'sleet', 'hail', 'clear'].

По сути, мы создали новый массив, извлекая элементы из существующего массива.

Мы определили функцию forecast, которая принимает массив в качестве аргумента. Измените функцию, используя slice()для извлечения информации из массива аргументов и возврата нового массива, содержащего строковые элементы warmи sunny.
### Before
```javascript
function forecast(arr) {
  // Only change code below this line

  return arr;
}

// Only change code above this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
```


### Answers
```javascript

```

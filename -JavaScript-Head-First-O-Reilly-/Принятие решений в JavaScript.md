# Принятие решений в JavaScript
```javascript
if (scoops < 3) { /*Ключевое слово if, за которым следует
условие и программный блок.Это условие проверяет, осталось ли меньше
трех шариков мороженого.*/
alert("Ice cream is running low!"); /*И если осталось меньше трех, выполняется
программный блок команды if.Функция alert получает строку и выводит
ее во всплывающем окне браузера. Попробуйте!*/
}


if (scoops >= 5) {
alert("Eat faster, the ice cream is going to melt!"); /*Сначала проверяется одно условие, если оно
не выполняется, то проверяется другое,
указанное в if/else:*/
} else if (scoops < 3) { /*Добавьте столько дополнительных проверок
“else if ”, сколько вам нужно; с каждым усло-
вием связывается свой программный блок,
выполняющийся в случае его истинности.*/
alert("Ice cream is running low!");
}
```

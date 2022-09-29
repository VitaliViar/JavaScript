# Цепочка операторов If Else
`if/else`операторы могут быть объединены в цепочку для сложной логики. Вот _псевдокод_ нескольких связанных операторов `if`/ :`else if`

```javascript

if (condition1) {
  statement1
} else if (condition2) {
  statement2
} else if (condition3) {
  statement3
. . .
} else {
  statementN
}
```
## Instructions

Напишите цепочку операторов `if`/ `else if`, чтобы выполнить следующие условия:

```javascript

num < 5- вернуться Tiny
num < 10- вернуться Small
num < 15- вернуться Medium
num < 20- вернуться Large
num >= 20- вернутьсяHuge
```
### Before

```javascript

function testSize(num) {
  // Only change code below this line


  return "Change Me";
  // Only change code above this line
}

testSize(7);
```
### Answers

```javascript

function testSize(num) {
  // Only change code below this line
if (num < 5) {
  return "Tiny";
} else if (num < 10) {
  return "Small";
} else if (num < 15) {
  return "Medium";
} else if (num < 20) {
  return "Large";
}else if (num >= 20) {
  return "Huge";

  // Only change code above this line
}}
```

# Понимание выражения немедленно вызываемой функции (IIFE)
Распространенным шаблоном в JavaScript является выполнение функции, как только она объявлена:
```javascript
(function () {
  console.log("Chirp, chirp!");
})();
```
Это выражение анонимной функции, которое выполняется сразу же и `Chirp`, `chirp!`немедленно выводит.

Обратите внимание, что функция не имеет имени и не хранится в переменной. Две круглые скобки `()` в конце функционального выражения заставляют его немедленно выполняться или вызываться. Этот шаблон известен как _немедленно вызываемое функциональное выражение_ или _IIFE_ .

Перепишите функцию `makeNest`и удалите ее вызов, чтобы вместо этого она представляла собой анонимное немедленно вызываемое функциональное выражение (IIFE).
### Before
```javascript
function makeNest() {
  console.log("A cozy nest is ready");
}

makeNest();
```
### Answers
```javascript
(function () {
  console.log("A cozy nest is ready");
})();
```

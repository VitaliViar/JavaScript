# Повторное использование кода JavaScript с помощью импорта
`import`позволяет выбрать, какие части файла или модуля загружать. В предыдущем уроке примеры экспортировались `add`из `math_functions.jsфайла`. Вот как вы можете импортировать его для использования в другом файле:
```javascript
import { add } from './math_functions.js';
```
Здесь `import`вы найдете `add`, `math_functions.js`импортируете только эту функцию для использования и проигнорируете остальные. Сообщает ./импорту искать `math_functions.js`файл в той же папке, что и текущий файл. Относительный путь к файлу (` ./`) и расширение файла ( `.js`) необходимы при использовании импорта таким образом.

Вы можете импортировать более одного элемента из файла, добавив их в `import`оператор следующим образом:
```javascript
import { add, subtract } from './math_functions.js';
```
## Instructions
Добавьте соответствующий `import`оператор, который позволит текущему файлу использовать функции `uppercaseString`и `lowercaseString`, которые вы экспортировали в предыдущем уроке. Эти функции находятся в файле с именем `string_functions.js`, который находится в том же каталоге, что и текущий файл.

  ### Before
  ```javascript
// Only change code above this line

uppercaseString("hello");
lowercaseString("WORLD!");

```
### Answers
```javascript
  import { uppercaseString, lowercaseString } from './string_functions.js';
// Only change code above this line

uppercaseString("hello");
lowercaseString("WORLD!");
```

# Преобразование объектов HTML
Преобразуйте символы `&`, `<`, `>`, "(двойные кавычки) и '(апостроф) в строке в соответствующие им объекты HTML.

### Before
```javascript
function convertHTML(str) {
  return str;
}

convertHTML("Dolce & Gabbana");
```
### Answers
```javascript
function convertHTML(str) {
    // Use Object Lookup to declare as many HTML entities as needed.
  const htmlEntities = {
    "&": "&amp;",
    "<": "&lt;",
    ">": "&gt;",
    '"': "&quot;",
    "'": "&apos;"
  };
  // Using a regex, replace characters with it's corresponding html entity
  return str.replace(/([&<>\"'])/g, match => htmlEntities[match]);
}

// test here

convertHTML("Dolce & Gabbana");
```

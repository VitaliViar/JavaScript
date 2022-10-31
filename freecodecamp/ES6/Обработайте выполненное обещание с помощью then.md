# Обработайте выполненное обещание с помощью then
Промисы наиболее полезны, когда у вас есть процесс, который занимает неизвестное количество времени в вашем коде (например, что-то асинхронное), часто запрос к серверу. Когда вы делаете запрос к серверу, это занимает некоторое время, и после его завершения вы обычно хотите что-то сделать с ответом от сервера. Этого можно добиться, используя `then`метод. Метод `then`выполняется сразу после того, как ваше обещание выполнено с помощью `resolve`. Вот пример:
```javascript
myPromise.then(result => {
  
});
```
`result`исходит из аргумента, данного `resolve`методу.
## Instructions
Добавьте `then`метод к вашему обещанию. Используйте `result`в качестве параметра его функцию обратного вызова и войдите `result`в консоль.

### Before
```javascript
const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to true to represent a successful response from a server
  let responseFromServer = true;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});
```
### Answers
```javascript
const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to true to represent a successful response from a server
  let responseFromServer = true;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});
makeServerRequest.then(result => {
  console.log (result);
});
```

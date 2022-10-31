# Обработка отклоненного обещания с помощью catch
`catch`это метод, используемый, когда ваше обещание было отклонено. Он выполняется сразу после вызова `reject`метода обещания. Вот синтаксис:
```javascript
myPromise.catch(error => {
  
});
```
`error`аргумент, передаваемый `reject`методу.
## Instructions
Добавьте `catch`метод к вашему обещанию. Используйте `error`в качестве параметра его функцию обратного вызова и войдите `error`в консоль.
### Before
```javascript
const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to false to represent an unsuccessful response from a server
  let responseFromServer = false;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});

makeServerRequest.then(result => {
  console.log(result);
});
```
### Answers
```javascript
const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to false to represent an unsuccessful response from a server
  let responseFromServer = false;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});

makeServerRequest.then(result => {
  console.log(result);
});
makeServerRequest.catch(error => {
  console.log (error);
});
```

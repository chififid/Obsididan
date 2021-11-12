---
type: paper
tags: 📥️/📜️/🩳 🖥️
aliases:
  - Async/await
---



# Title: **[[Async-await 2021-11-02]]**
- `Type:` [[&]]
- `Links:` [[Promise 2021-11-02|Promise]]
- `Reviewed Date:` [[2021-11-02]]

```javascript
const getFirstUserData = async () => {
 const response = await fetch('/users.json') // get users list
 const users = await response.json() // parse JSON
 const user = users[0] // pick first user
 const userResponse = await fetch(`/users/${user.name}`) // get user data
 const userData = await userResponse.json() // parse JSON
 return userData
}
```
Что-бы не городить then в вашем коде, просто добавь async при создании функции и поставь await перед промисами которых нужно дождаться. Любая async функция возвращает [[Promise 2021-11-02|промис]], хотя это никак не мишает использовать возвращаемое значение как просто значение. Async/await построенна внутри на промисах.
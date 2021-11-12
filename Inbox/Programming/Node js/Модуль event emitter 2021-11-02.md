---
type: paper
tags: 📥️/📜️ 🖥️
aliases:
  - Модуль event emitter node js
---



# Title: **[[Модуль event emitter 2021-11-02]]**


## Metadata:

- `Type:` [[&]]
- `Links:` [[Асинхронность 2021-11-02|Асинхронность и Node js]], [[Event loop 2021-11-02|Event loop Node js]]
- `Author:` 
	- `Notable Authors:` 
- `Keywords:` [[Коллбек]], [[Событие]]
- `Specific Subject:` [[Модули]]
- `General Subject:` [[Node js 2021-10-18|Node js]]
- `Reviewed Date:` [[2021-11-02]]

## Notes
### Идея
```javascript
const EventEmitter = require('events')
const eventEmitter = new EventEmitter()

eventEmitter.on('start', () => {
 console.log('started')
})
eventEmitter.emit('start')
```
EventEmitter - модуль, [[Асинхронность 2021-11-02|асинхронный]] подписчик на событие, вызывающий [[Event loop 2021-11-02#Коллбеки|коллбек]].

### Методы
```javascript
eventEmitter.once('start', () => {
 console.log('started')
}) // 1
eventEmitter.removeListener('start', something) // 2
eventEmitter.removeAllListeners('start') // 3
```
1) Добавить единожды работающий event.
2) Удалить какой-то коллбек.
3) Удалить все коллбеки.
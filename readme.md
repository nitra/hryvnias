# hryvnias.js — Вартість прописом

Форк корисного пакету [rubles](//www.npmjs.com/package/rubles)

В українському документообігу прийнято писати суму літерами. Таке повинно бути в договорах, актах, розписках та інших подібних документах. hryvnias.js покликаний вирішити цю проблему комплексно, він працює в браузері і на стороні сервера.

### На сервері

#### Встановити через [npm](//npmjs.org)

```bash
$ npm i --save hryvnias
```

#### Як використовувати

```js
var hryvnias = require('hryvnias').rubles

// Якщо ми хочемо просто отримати число прописом
var text = hryvnias(52151, true)
console.log(text) // п'ятдесят дві тисячі сто п'ятдесят один

// А якщо з грошами
var text = hryvnias(12.1)
console.log(text) // дванадцять гривень 10 копійок

var text = hryvnias('52151,31')
console.log(text) // п'ятдесят дві тисячі сто п'ятдесят один гривня 31 копійка
```

---

### В браузері

#### Встановити через [bower](http://bower.io)

```bash
$ bower install hryvnias --save
```

#### Як підключити

```html
<script src="bower_components/hryvnias/lib/hryvnias.min.js"></script>
```

#### Як використовувати

```html
<script>
  var text = rubles(12.1)
  console.log(text) // дванадцять гривень 10 копійок

  var text = rubles('52151,31')
  console.log(text) // п'ятдесят дві тисячі сто п'ятдесят один гривня 31 копійка
</script>
```

---

## Автор

- [Олексій Симоненко](mailto:alexey@simonenko.su), [simonenko.su](http://simonenko.su)

## Ліцензія

Ліцензія MIT, дивіться файл `license.md`.

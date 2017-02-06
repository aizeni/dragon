# dragon
dragon es un pequeño motor de plantilla, que consta de funcionales como control de flujo, incluir y extender plantillas, manejando la indentacion al abrir y cerrar etiquetas dragon. funciona tanto como para [Node.js](https://nodejs.org) y navegadores
# Installation
via npm
```bash
$ npm install dragon-engine
```
# Syntax
the dragon templates are handled by indentation
```html
<div>
    <? if str instanceof String ?>
        <p>my indented content</p>
    <? else ?>
        <p>not string</p>
    <? endif ?>
</div>
```
output
```html
<div>
        <p>my indented content</p>
</div>
```

# Usage
```js
var html = dragon.compile(/*html*/'<?= str ?>', /*data*/ {
    str: 'hello'
});
```
# License
MIT
# TextMarker

If you have only the initial and final piece of text that should be marked (highlighted) in an HTML, this project is what you need ;)

Check the example in respective folder.

## Basic usage

Given the following `HTML`:

```html
<div class=".body">
    <p>My text to be completely marked! Another text.</p>
    <p>Another paragraph that have no mark.</p>
</div>
```
When you use the script here:

```javascript
// .body is a selector
var instance = new TextMarker('.body');
instance.mark('My text', 'completely marked');
```

The `HTML` will be updated to:

```html
<div class=".body">
    <p><mark data-marked="true">My text</mark><mark data-marked="true"> to be</mark><mark data-marked="true"> completely marked</mark>! Another text.</p>
    <p>Another paragraph that have no mark.</p>
</div>
```

## Credits

This project depends on MarkJS project, by Julian Kühnel, available on https://markjs.io/.

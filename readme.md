# Picker

"Pickier" select form controll.

## Dependencies

1. [list.js](https://github.com/javve/list.js)
2. [list.fuzzysearch.js](https://github.com/javve/list.fuzzysearch.js)
3. [Bourbon](https://github.com/thoughtbot/bourbon)

## Installation

1. Add `picker.js` to your build workflow.
2. Add `picker.scss` to your build workflow.
3. Add all files in `images` directory to your build workflow.
4. Update all `url()` paths in `picker.scss` to the directory you moved the `images/*` to.
5. Add `class="picker"` to the `<select>`.
5. Initialize the picker in your main `.js` file:

```js
var pickers = document.getElementsByClassName('picker');
for (var i = pickers.length - 1; i >= 0; i--) {
    var picker = new Picker(pickers[i]);
    picker.init();
};
```
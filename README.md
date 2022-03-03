## How to Use
### HTML
```HTML
<script src="https://raw.githubusercontent.com/jc3213/filereader.js/main/filereader.js"
        integrity="sha256-t3P/rX1FsOwYp2VrKhwqzimi9ANGJKTGDjHFICmvTvY=" crossorigin="anonymous"></script>
```
### TamperMonkey
```javascript
// @require https://raw.githubusercontent.com/jc3213/filereader.js/main/filereader.js#sha256-t3P/rX1FsOwYp2VrKhwqzimi9ANGJKTGDjHFICmvTvY=
```
## Syntax
```javascript
const reader = new PromiseFileReader(file);
```
### `file`
A javascript File object
## Method
### `reader.text()`
Return a promise object, which returns the contents of the file as a text `string` if fulfilled
### `reader.data()`
Return a promise object, which returns a `data:` URL representing the file's data if fulfilled
### `reader.buffer()`
Return a promise object, which returns an `ArrayBuffer` representing the file's data if fulfilled
### `reader.binary()`
Return a promise object, which returns the raw binary data from the file as a `string` if fulfilled

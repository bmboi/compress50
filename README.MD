<h1>Compress50</h1>
a compression library that i tried to use to replace LZ78, using my own algorithm
<br>
<h3>Usage</h3>
html:

```html
<script src="https://raw.githubusercontent.com/bmboi/compress50/main/index.js"></script>
```
in your scripts:

```js
console.log('Compressed: '+Compress50.compress('String compression is really cool!')); // ᑅ♌➌7⟒♄
console.log('Decompressed: '+Compress50.decompress('᧔⥉❇C⟍⡒⋓⧉⟎I⦀⥅⃌♙C⟏☁')) // String compression is really cool!

//Test for data loss
console.log(`Saved ${50/(Compress50.compress('String compression is really cool!').split('').length/Compress50.decompress(Compress50.compress('String compression is really cool!')).split('').length)}%, lost ${(50/(Compress50.compress('String compression is really cool!').split('').length/Compress50.decompress(Compress50.compress('String compression is really cool!')).split('').length))-100}%`)
```

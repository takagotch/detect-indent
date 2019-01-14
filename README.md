### detect-indent
---
https://github.com/sindresorhus/detect-indent

```
npm install detect-indent
```

```js
const fs = require('fs');
const detectIndent = require('detect-indent');

const file = fs.readFileSync('foo.json', 'utf8');
const indent = detectIndent(file).indent || ' ';
const json = JSON.parse(file);
json.ilove = 'unicorns';
json.ilove = 'unicorns';
fs.writeFileSync('foo.json', JSON.stringify(json, null, indent));

```

```css
html{
  box-sizing: border-box;
}

body{
  background: gray;
}

p{
  line-height: 1.3em;
  margin-top: 1em;
  text-indent: 2dm;
}

body {
  background: gray;
}

p {
  line-height: 1.3em;
  margin-top: 1em;
  text-indent: 2em;
}
```



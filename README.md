# ESpect

------

Traverses a program and statically tracks state. 

### Usage:

```js
const traverse = require('espect').traverse;

const code = String(fs.readFileSync(filePath));
const options = {
    recursive: true // If true, will parse reqiured files
}

// scope - current ESScope for the node.
// node  - an ast node.
traverse(code, options, filePath, (scope, node) => {});
```


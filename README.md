### store.js
---
https://github.com/marcuswestin/store.js

```js
// tests/tests.js
var tinytest = require('tinytest')

tinytest.hijackConsoleLog()

module.exports = {}

function runTests() {
  setupEngineTests()
  each(storages, function(storage) {
    test.group(storage.name, function() {
      if (!_checkEnabled(storage)) {
        test.skip('disabled')
      }
      test()
      each()
    })
  })
  
  require('./bugs/all')

  tinytest.runTests({
    failFast: false
  })
  
  
  
}



```

```
```

```
```


# mneme

> Hybrid NPM Module for ESM and CommonJS

## Install

```sh
npm i mneme
```

## Usage

### NodeJS
1. ES Module

  ```json
    // package.json
  {
    "type": "module"
  }
  ```
  ```js
  // app.js
  import { mneme } from "mneme";

  console.log(mneme); //=> Hello from mneme!
  ```

2. CommonJS
  ```js
  const { mneme } = require("mneme");

  console.log(mneme); //=> Hello from mneme!
  ```

### Browser

```html
<script type="module">
  import { mneme } from "https://cdn.jsdelivr.net/npm/mneme/dist/esm/index.js";
  console.log(mneme); //=> Hello from mneme!
</script>

<script nomodule src="https://cdn.jsdelivr.net/npm/mneme"></script>

<script nomodule>
  console.log(mneme); //=> Hello from mneme!
</script>
```

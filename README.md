# ESLint + Prettier config for NodeJS applications

We use both eslint and prettier to lint our code:

* eslint is for code-quality.
* prettier is for formatting.

## Installation

```sh
yarn add --dev @gazzati/eslint-config-node
```

also add `eslint` if not already added
```
yarn add --dev eslint
```

Extend the shared eslint config in `.eslintrc.js`:

```js
// .eslintrc.js

module.exports = {
  extends: ["@gazzati/eslint-config-node"],
  rules: {
    // Specific project rules
  },
};
```

Extend the shared prettier config in `.prettierrc.js`:

```js
// .prettierrc.js

module.exports = require('@gazzati/eslint-config-node/.prettierrc')
```
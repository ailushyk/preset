# Nodejs + typescript

```sh
pnpm add -D eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin prettier eslint-config-prettier
```


## ESlint

```json
{
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaVersion": 12,
    "sourceType": "module"
  },
  "plugins": ["@typescript-eslint"],
  // HERE
  "extends": ["eslint:recommended", "plugin:@typescript-eslint/recommended", "prettier"],

  "rules": {
    "@typescript-eslint/no-unused-vars": "error",
    "@typescript-eslint/consistent-type-definitions": ["error", "type"]
  },

  "env": {
    "browser": true,
    "es2021": true
  }
}
```

## Prettier

```json
{
  "singleQuote": true,
  "semi": false
}
```

# Prettier and ESlint

## Install

- eslint
- prettier
- prettier eslint config
- organize [imports](https://github.com/simonhaenisch/prettier-plugin-organize-imports?tab=readme-ov-file)
- tailwindcss [plugin](https://github.com/tailwindlabs/prettier-plugin-tailwindcss)

```sh
pnpm add -D eslint prettier eslint-config-prettier prettier-plugin-organize-imports prettier-plugin-tailwindcss
```

## Prettier

add `.prettierrc.json` config file:

```json
{
  "singleQuote": true,
  "semi": false
}
```

add plugins

```json
{
  // ...
  "plugins": [
    "prettier-plugin-organize-imports",
    "prettier-plugin-tailwindcss"
  ]
}
```

## ESlint

Add eslint-config-prettier to your ESLint configuration `.eslintrc.json`

```json
{
  "extends": [
    "next/core-web-vitals", 
    "prettier"
  ]
}
```

add react rules

```json
{
  // ...
  "rules": {
    "react/self-closing-comp": [
      "error",
      {
        "component": true,
        "html": true
      }
    ],
    "react/jsx-curly-brace-presence": [
      "error",
      {
        "props": "never",
        "children": "never"
      }
    ]
  }
}
```

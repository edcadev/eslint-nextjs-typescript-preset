This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, install the dependencies

```bash
npm install
# or
yarn add
```

Second, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

Now you can start editing the project. The page auto-updates as you edit the file.

To configure the EsLint rules, just copy the following code into the `.eslintrc` file.

```json
{
  "root": true,
  "env": {
    "browser": true,
    "es2021": true,
    "node": true
  },
  "extends": [
    "next/core-web-vitals",
    "plugin:react/recommended",
    "airbnb",
    "airbnb-typescript",
    "plugin:@typescript-eslint/recommended",
    "plugin:@typescript-eslint/recommended-requiring-type-checking",
    "plugin:@typescript-eslint/strict",
    "plugin:react/jsx-runtime",
    "prettier"
    // "plugin:prettier/recommended", // Optional
  ],
  "overrides": [],
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module",
    "tsconfigRootDir": "./",
    "project": ["./tsconfig.json"]
  },
  "plugins": ["react", "react-hooks", "@typescript-eslint", "prettier"],
  "rules": {
    // Checks rules of Hooks
    "react-hooks/rules-of-hooks": "error",
    // Checks effect dependencies
    "react-hooks/exhaustive-deps": "warn",
    "react/jsx-props-no-spreading": [
      "error",
      {
        "custom": "ignore"
      }
    ],
    "prettier/prettier": "error"
  },
  "settings": {
    "react": {
      "version": "detect"
    }
  }
}
```

To configure the Prettier rules, just copy the following code into the `.prettierrc` file.

```json
{
  "printWidth": 80,
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true,
  "jsxSingleQuote": true,
  "trailingComma": "all",
  "bracketSpacing": true,
  "bracketSameLine": true,
  "arrowParens": "always",
  "endOfLine": "lf",
  "singleAttributePerLine": true
}
```

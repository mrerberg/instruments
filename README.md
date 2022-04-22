# Instruments

## Prettier

Code formatting tool.

Install package:

```bash
npm install --save-dev prettier
```

Create config file and add some rules to config file. See all rules [here](https://prettier.io/docs/en/options.html).

```text
.prettierrc.{yml,json}
```

Add formatting script to your package.json file

```json
{
    "format": "prettier --write ."
}
```

Add `.prettierignore` file to exclude some files from formatting

## [Eslint](https://eslint.org/)

JS code linting tool.

Install package:

```bash
npm install --save-dev eslint-plugin-prettier eslint-config-prettier
```

Create config file and add some rules to config file. See all rules [here](https://eslint.org/docs/rules/).

```text
.eslintrc.{yml,json,js}
```

Add `.eslintignore` file to exclude some files from linting

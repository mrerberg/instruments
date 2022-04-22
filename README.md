# Tools

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

Add linting script to your package.json file

```json
{
    "lint:js": "eslint '**/*.js'"
}
```

Add `.eslintignore` file to exclude some files from linting

## [Stylelint](https://stylelint.io/)

Css (scss, sass, less) code linting tool.

Install package:

```bash
npm install --save-dev stylelint stylelint-config-standard stylelint-config-prettier stylelint-prettier
```

Create config file and add some rules to config file. See all rules [here](https://stylelint.io/user-guide/rules/list).

```text
.stylelintrc.{yml,json,js}
```

Add linting script to your package.json file

```json
{
    "lint:css": "stylelint './src/**.css'"
}
```

## [Husky](https://typicode.github.io/husky/#/)

Tool for running scripts with git hooks.

Install package:

```bash
npm install -D husky
```

Add script to your package.json file and run it

```json
{
    "prepare": "husky install"
}
```

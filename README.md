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

### SCSS

Install package:

```bash
npm install --save-dev stylelint-scss stylelint-config-standard-scss
```

Add package to stylelint config `plugins`:

```yml
plugins: ['stylelint-scss']
```

Add overrides to stylelint config:

```yml
overrides: [{ files: ['**/*.scss'], customSyntax: 'postcss-scss' }]
```

Add linting script to your package.json file

```json
{
    "lint:scss": "stylelint './src/**.scss'"
}
```

Add to VSCode editor settings:

```json
{
  "stylelint.validate": ["css", "scss"],
}
```

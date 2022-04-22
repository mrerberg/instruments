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

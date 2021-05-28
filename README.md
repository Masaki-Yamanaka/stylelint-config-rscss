# stylelint-config-rscss

Configuration of Stylelint for RSCSS

## Usage

```bash
# Install dependencies
yarn add -D stylelint stylelint-scss stylelint-config-recommended-scss stylelint-config-recess-order stylelint-rscss stylelint-config-prettier
```

- Copy stylelint.config.js .stylelintignore
- Add following scripts in package.json

```bash
"scripts": {
  "lint:scss": "stylelint \"**/*.{vue,scss,css}\"",
  "lint:scss:fix": "stylelint --fix \"**/*.{vue,scss,css}\""
}
```

### Prettier

Since turned off all rules that might conflict with Prettier, please make sure Prettier is installed.

```bash
# Install dependencies
yarn add -D prettier
```

- Copy .prettierrc
- Add following scripts in package.json

```bash
"scripts": {
  "format:scss": "prettier -c (directory)",
  "format:scss:fix": "prettier -w (directory)"
}
```

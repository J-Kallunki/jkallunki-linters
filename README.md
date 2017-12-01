# jkallunki-react-vscode
Basic prettier and linter setup for VScode React projects
[Prettier](https://github.com/prettier/prettier)
[ESlint](https://github.com/eslint/eslint) using [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)  
[Stylelint](https://github.com/stylelint/stylelint) usfin [Airbnb CSS / Sass Styleguide](https://github.com/airbnb/css)

## On project
`yarn global add stylelint`  
`yarn add --dev babel-eslint prettier-eslint`

Add stylelint script to package.json scripts:
```
"scripts": {
  "stylelint": "stylelint '**/*.scss'; exit 0"
}
```

## VScode plugins
* [esbenp.prettier-vscode](https://github.com/prettier/prettier-vscode)
* [dbaeumer.vscode-eslint](https://github.com/Microsoft/vscode-eslint)
* [dzannotti.vscode-babel-coloring](https://github.com/dzannotti/vscode-babel)
* [shinnn.stylelint](https://github.com/shinnn/stylelint-vscode)

## VScode settings
Open settings via __CMD + ,__ and add there:
```
{
  "files.autoSave": "off",
  // Format a file on save. A formatter must be available, the file must not be auto-saved, and editor must not be shutting down.
  "editor.formatOnSave": true,
  // Enable/disable default JavaScript formatter (For Prettier)
  "javascript.format.enable": false,
  // Use 'prettier-eslint' instead of 'prettier'. Other settings will only be fallbacks in case they could not be inferred from eslint rules.
  "prettier.eslintIntegration": true,
  "stylelint.enable": true,
  "css.validate": false,
  "scss.validate": false
}
```

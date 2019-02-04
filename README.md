# style-guide

Set of configs (ESLint, Editorconfig, Prettier) to use on my own projects.

## ESLint

```json
{
  "parser": "babel-eslint",
  "env": {
    "browser": true,
    "jest": true
  },
  "plugins": ["react", "jsx-a11y", "import"],
  "extends": "airbnb",
  "rules": {
    "comma-dangle": ["error", "always-multiline"],
    "consistent-return": [0],
    "global-require": "off",
    "import/prefer-default-export": "off",
    "jsx-quotes": ["error", "prefer-single"],
    "no-unused-expressions": ["error", { "allowTaggedTemplates": true }],
    "no-use-before-define": ["nofunc"],
    "react/jsx-filename-extension": ["error", { "extensions": [".js", ".jsx"] }],
    "react/jsx-one-expression-per-line": [0],
    "semi": ["error", "never"]
  }
}
```

## Editorconfig

```editorconfig
root = true

[*]
indent_style = space
indent_size = 2
charset = utf-8
end_of_line = lf
trim_trailing_whitespace = true
insert_final_newline = true
```

## VSCode Prettier Settings

```json
{
  "prettier.arrowParens": "always",
  "prettier.eslintIntegration": true,
  "prettier.jsxSingleQuote": true,
  "prettier.printWidth": 90,
  "prettier.semi": false,
  "prettier.singleQuote": true,
  "prettier.trailingComma": "es5"
}
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

[MIT License](http://iagodahlem.mit-license.org/) © Iago Dahlem

# style-guide

Set of configs (ESLint, Editorconfig, Prettier) to use on my own projects.

## Plugins

```sh
yarn add -D \
  eslint-config-airbnb \
  eslint-plugin-cypress \
  eslint-plugin-import \
  eslint-plugin-jsx-a11y \
  eslint-plugin-react
```

## ESLint

```json
{
  "parser": "babel-eslint",
  "env": {
    "browser": true,
    "jest": true,
    "cypress/globals": true
  },
  "plugins": ["react", "jsx-a11y", "import", "cypress"],
  "extends": ["airbnb", "react-app", "plugin:cypress/recommended"],
  "rules": {
    "arrow-parens": ["error", "as-needed"],
    "semi": ["error", "never"],
    "comma-dangle": ["error", "always-multiline"],
    "consistent-return": [0],
    "no-use-before-define": [0],
    "global-require": "off",
    "import/no-unresolved": "off",
    "import/prefer-default-export": "off",
    "react/jsx-filename-extension": ["error", { "extensions": [".js", ".jsx"] }],
    "jsx-quotes": ["error", "prefer-single"],
    "react/jsx-one-expression-per-line": [0],
    "no-unused-expressions": ["error", { "allowTaggedTemplates": true }],
    "object-curly-newline": ["error", { "consistent": true }]
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

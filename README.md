# vscode-config

### Install Eslint with airbnb dependencies
* First step install _Eslint and Prettier - Code Formater_ extensions from the store on VS CODE
* Then run this command on root folder
```
npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node
```
* This one too:
```
npx install-peerdeps --dev eslint-config-airbnb
```

* Create a new file configuration:
 * Create a file named *.prettierrc*
 then type:
 ```
{
  "singleQuote": true,
  "trailingComma": "es5"
}
 ```
 * And save. After this run the command below in root folder
 ```
 sudo npm i -g eslint
 ```
 * Type eslint --init in terminal to configurate file and choose the options below (can be other depending on your project)
 To check syntax and find problems;
 JavaScript modules(import/export) --> React, view;
 CommonJS --> Node.JS
 
* After all choices, will create a file named .eslintrc.json. Open it and overwrite with command below
```
{
  "env": {
    "es6": true,
    "node": true,
    "jest": true
  },
  "extends": ["airbnb-base", "prettier"],
  "plugins": ["prettier"],
  "globals": {
    "Atomics": "readonly",
    "SharedArrayBuffer": "readonly",
    "console": "readonly",
    "process": "readonly",
    "Buffer": "readonly",
    "expect": "readonly",
    "describe": "readonly",
    "it": "readonly"
  },
  "parserOptions": {
    "ecmaVersion": 2018,
    "sourceType": "module"
  },
  "rules": {
    "prettier/prettier": "error",
    "class-methods-use-this": "off",
    "no-param-reassign": "off",
    "no-use-before-define": "off",
    "no-await-in-loop": "off",
    "no-restricted-syntax": "off",
    "no-console": "off",
    "camelcase": "off",
    "no-unused-vars": [
      "error",
      {
        "argsIgnorePattern": "next"
      }
    ]
  }
}
```

### Settings.json
* Type Ctrl + Shift + P then type **Open Settings (JSON)**
Changes:
```
  {
  "workbench.startupEditor": "newUntitledFile",
  "editor.formatOnPaste": true,
  "editor.formatOnSave": true,
  "workbench.editor.highlightModifiedTabs": true,
  "editor.mouseWheelZoom": true,
  "editor.suggestSelection": "first",
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "workbench.editor.enablePreview": false,
  "workbench.editor.enablePreviewFromQuickOpen",
}
```
### Customization
* Material Icon Themes

### Packages
* Bracket Pair Colorizer
* Path Intellisence
* Visual Studio Intellicode
* Git Lens
* Better Comments
* Debugger for Chrome


### Shortcuts!
Alt + Up or Down --> Change line position
Alt + Shift + Up or Down --> Duplicate line or selection

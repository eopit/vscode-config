# vscode-config

### Install Eslint with airbnb dependencies
* First step install _Eslint and Prettier - Code Formater_ extensions
```
npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node
```
* Then run in root folder:
```
npx install-peerdeps --dev eslint-config-airbnb
```

* Create file configurations:
 *Create a file named *.prettierrc*
 then type:
 ```
 {
  "singleQuote": true
 }
 ```
 * And save. After this, run the command below in root folder
 ```
 sudo npm i -g eslint
 ```
 * Type eslint --init in terminal to configurate file
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
  * "editor.formatOnPaste": true 
  * "editor.formatOnSave": true
  * "workbench.editor.highlightModifiedTabs": true
  *  "editor.cursorStyle": "block"  --> block, block-outline, line, line-thin, underline, or underline-thin
  * "editor.cursorBlinking": "smooth" --> blink, smooth, phase, expand, or solid
  * "editor.mouseWheelZoom": true,
  
  
### Customization
* Material Icon Themes


### Packages
* Bracket Pair Colorizer
* Path Intellisence
* Visual Studio Intellicode
* Git Lens
* Better Comments




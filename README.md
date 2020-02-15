# vscode-config

### Install Eslint with airbnb dependencies

* First step install eslint in the node root folder:
```
npm install eslint eslint-config-airbnb-base eslint-plugin-import -d
```
* Create a file called ".eslintrc.js" in the root folder then export the module typing:
```
module.exports={
 "extends" : "airbnb-base"
}
```
* Then open the extension page with **Ctrl + Shift + x** then search for EsLint and download the recommended extension then restart vsCode.

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




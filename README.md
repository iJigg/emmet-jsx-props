# emmet-jsx-props package

Atom package to extend Emmet's JSX expansions to convert string attributes to js props

## Demo
![alt tag](https://github.com/iJigg/emmet-jsx-props/raw/master/demo.gif)

## Enable tab completion for JSX with Emmet in Atom
This guide assumes you have the emmet and language-babel packages already installed in Atom

1. Open the keymap.cson file by clicking on Atom -> Keymap… in the menu bar
2. Add these lines of code to your keymap:
```
'atom-text-editor[data-grammar~="jsx"]:not([mini])':
  'tab': 'emmet:expand-abbreviation-with-tab'
```

Now open a file with JSX code, type div[prop=myProp], press tab and it should autocomplete to `<div prop={myProp}></div>`! (if it's not properly syntax highlighted, select Babel ES6 JavaScript or JSX as the syntax, this won't work otherwise)

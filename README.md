# My VS Code Setup

### Setings.json

```
{
  // editor
  "editor.fontSize": 22,
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "editor.wordWrap": "on",
  "editor.minimap.enabled": false,
  "editor.tokenColorCustomizations": {
    "comments": "#adacac",
    "functions": "#38ff59",
    "strings": "#ffffff",
    "keywords": "#f1ff2e",
    "variables": "#41bef8",
    "textMateRules": [
      {
        "scope": "comment",
        "settings": {
          "fontStyle": "italic"
        }
      },

      {
        "scope": "keyword",
        "settings": {
          "fontStyle": "bold",
          "foreground": "#ff30f5"
        }
      }
    ]
  },
  // cursor
  "editor.cursorSmoothCaretAnimation": true,
  "editor.cursorBlinking": "expand",
  // config related to code formatting
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.tslint": true,
    "source.organizeImports": true
  },
  "eslint.alwaysShowStatus": true,
  //terminal
  "terminal.integrated.fontSize": 16,
  "terminal.integrated.fontWeight": "normal",
  "terminal.integrated.fontFamily": "Fira Code, Sans",
  "workbench.iconTheme": "vscode-icons",
  "terminal.integrated.cursorBlinking": true,
  // terminal customization
  "workbench.colorCustomizations": {
    "terminal.background": "#000000",
    "terminal.foreground": "#ffffff",
    "terminalCursor.background": "#000000",
    "terminalCursor.foreground": "#23ff3c",
    "terminal.ansiBlack": "#000000",
    "terminal.ansiBlue": "#46c7ff",
    "terminal.ansiBrightBlack": "#000000",
    "terminal.ansiBrightBlue": "#38ff06",
    "terminal.ansiBrightCyan": "#2acaff",
    "terminal.ansiBrightGreen": "#ff04d5",
    "terminal.ansiBrightMagenta": "#ff5bd9",
    "terminal.ansiBrightRed": "#ff4343",
    "terminal.ansiBrightWhite": "#F7F7F7",
    "terminal.ansiBrightYellow": "#FDED02",
    "terminal.ansiCyan": "#B5E4F4",
    "terminal.ansiGreen": "#01A252",
    "terminal.ansiMagenta": "#A16A94",
    "terminal.ansiRed": "#ff3b2d",
    "terminal.ansiWhite": "#A5A2A2",
    "terminal.ansiYellow": "#FDED02",
    "terminalCommandDecoration.defaultBackground": "#1dff51",
    "terminal.border": "#39ff39",

    "[2077]": {
      "activityBar.border": "#00ff2a",
      "activityBar.activeBackground": "#16cc2b",
      "editor.background": "#000000",
      "sideBar.background": "#000000",
      "sideBar.border": "#00ff2a",
      "statusBar.background": "#000550",
      "statusBar.foreground": "#ffffff",
      "activityBar.foreground": "#ffffff",
      "breadcrumb.background": "#0d1133",
      "breadcrumb.foreground": "#ffffff",
      "breadcrumb.focusForeground": "#2cf53c",
      "editorLineNumber.foreground": "#3cfcdc",
      "editorLineNumber.activeForeground": "#ff3cf8",
      "icon.foreground": "#3cfd3c",
      "tab.activeBackground": "#0c0661",
      "tab.activeBorder": "#5bff31",
      "panel.background": "#030449",
      "panelTitle.activeForeground": "#4fff38",
      "panelTitle.inactiveForeground": "#ffffff",
      "panel.border": "#82ff2f"
    }
  },
  "editor.lineNumbers": "on",
  "files.autoSave": "afterDelay",
  "editor.multiCursorModifier": "ctrlCmd",
  "workbench.colorTheme": "2077"
}






```

## Extension

1. Auto Rename Tag
2. Bracket Pair Color Dwl
3. Code Runner
4. 2077 theme
5. Es7+ React/Redux/React-Native Snippets
6. ESLint
7. Live Server
8. Path Autocomplete
9. Prettier
10. Tailwind CSS Intellisense
11. Turbo Console Log
12. Vs Code Icon


## Install DevDependencies

```

yarn add -D eslint prettier

```

```

npx install-peerdeps --dev eslint-config-airbnb-base

```

```

yarn add -D eslint-config-prettier eslint-plugin-prettier

```



## Setup Linting Configuration file

Create a <b>.eslintrc.json</b> file in the project root and enter the below contents:

```

{
  "extends": ["prettier", "airbnb-base"],
  "parserOptions": {
    "ecmaVersion": 12
  },
  "env": {
    "commonjs": true,
    "node": true
  },
  "rules": {
    "no-console": 0,
    "indent": 0,
    "linebreak-style": 0,
    "prettier/prettier": [
      "error",
      {
        "trailingComma": "es5",
        "singleQuote": true,
        "printWidth": 100,
        "tabWidth": 4,
        "semi": true
      }
    ]
  },
  "plugins": ["prettier"]
}

```





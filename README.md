# My VS Code Setup

### Setings.json

`{
  // editor
  "editor.fontSize": 18,
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "editor.wordWrap": "on",
  "editor.minimap.enabled": false,
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": "comment",
        "settings": {
          "fontStyle": "italic"
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
  // terminal customization
  "workbench.colorCustomizations": {
    "terminal.background": "#090300",
    "terminal.foreground": "#a7f369",
    "terminalCursor.background": "#000000",
    "terminalCursor.foreground": "#00ff2a",
    "terminal.ansiBlack": "#090300",
    "terminal.ansiBlue": "#01A0E4",
    "terminal.ansiBrightBlack": "#5C5855",
    "terminal.ansiBrightBlue": "#01A0E4",
    "terminal.ansiBrightCyan": "#B5E4F4",
    "terminal.ansiBrightGreen": "#01A252",
    "terminal.ansiBrightMagenta": "#A16A94",
    "terminal.ansiBrightRed": "#DB2D20",
    "terminal.ansiBrightWhite": "#F7F7F7",
    "terminal.ansiBrightYellow": "#FDED02",
    "terminal.ansiCyan": "#B5E4F4",
    "terminal.ansiGreen": "#01A252",
    "terminal.ansiMagenta": "#A16A94",
    "terminal.ansiRed": "#DB2D20",
    "terminal.ansiWhite": "#A5A2A2",
    "terminal.ansiYellow": "#FDED02",
    "terminalCommandDecoration.defaultBackground": "#ff0000",
    "[Dracula]": {
      "activityBar.border": "#00ff2a",
      "activityBar.activeBackground": "#000",
      "editor.background": "#000000",
      "sideBar.background": "#04041b",
      "sideBar.border": "#00ff2a",
      "editor.lineHighlightBorder": "#00ff2a",
      "statusBar.background": "#0d1133",
      "statusBar.foreground": "#fff",
      "activityBar.foreground": "#ffffff",
      "breadcrumb.background": "#0d1133",
      "breadcrumb.foreground": "#00ff2a",
      "breadcrumb.focusForeground": "#ff0000"
    }
  },
  "workbench.colorTheme": "Dracula",
  "editor.lineNumbers": "relative",
  "window.zoomLevel": -1,
  "files.autoSave": "afterDelay",
  "editor.multiCursorModifier": "ctrlCmd"
}

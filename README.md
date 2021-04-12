# OM Extension Pack

## Extensions included on "om-extension-pack"

- CSS Formatter - [aeschli.vscode-css-formatter](https://marketplace.visualstudio.com/items?itemName=aeschli.vscode-css-formatter)
- Apollo GraphQL - [apollographql.vscode-apollo](https://marketplace.visualstudio.com/items?itemName=apollographql.vscode-apollo)
- Bracket Pair Colorizer 2 - [CoenraadS.bracket-pair-colorizer-2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2)
- ESLint - [dbaeumer.vscode-eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- EditorConfig for VS Code - [EditorConfig.EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
- Code Runner - [formulahendry.code-runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- vscode-styled-components - [jpoissonnier.vscode-styled-components](https://marketplace.visualstudio.com/items?itemName=jpoissonnier.vscode-styled-components)
- colorize - [kamikillerto.vscode-colorize](https://marketplace.visualstudio.com/items?itemName=kamikillerto.vscode-colorize)
- Git Graph
 - [mhutchie.git-graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
- Docker - [ms-azuretools.vscode-docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
- Python - [ms-python.python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- Jupyter (Python extension depends on it) - [ms-toolsai.jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- Reload - [natqe.reload](https://marketplace.visualstudio.com/items?itemName=natqe.reload)
- Om Theme (A Darker Dracula Theme) - [omthemes.omthemes](https://marketplace.visualstudio.com/items?itemName=omthemes.omthemes)
- Material Icon Theme - [PKief.material-icon-theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- YAMLPreview - [redhat.vscode-yaml](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
- Live Server - [ritwickdey.LiveServer](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- Code Spell Checker - [streetsidesoftware.code-spell-checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
- Brazilian Portuguese - Code Spell Checker - [streetsidesoftware.code-spell-checker-portuguese-brazilian](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker-portuguese-brazilian)
- Visual Studio IntelliCode - [VisualStudioExptTeam.vscodeintellicode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)

## settings.json

Some settings I like to use:

### Eslint:

```json
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": true,
  "source.fixAll": true
},
```

### Python:

```json
"python.linting.pylintArgs": [
  "--load-plugins=pylint_django",
  "--errors-only",
],
"[python]": {
  "editor.tabSize": 4,
  "editor.insertSpaces": true,
  "editor.formatOnSave": true,
  "editor.formatOnType": true
},
"python.pythonPath": "/bin/python3.8",
"python.linting.flake8Enabled": true,
"python.linting.mypyEnabled": true,
"python.testing.unittestEnabled": true,
"files.associations": {
  "*.html": "html",
  "**/templates/*.html": "django-html",
  "**/templates/*": "django-txt",
  "**/requirements{/**,*}.{txt,in}": "pip-requirements"
},
```

### Bracket Pair Colorizer 2:

```json
"bracket-pair-colorizer-2.colors": [
  "#8BE9FD",
  "#50FA7B",
  "#FFB86C",
  "#FF79C6",
  "#BD93F9",
  "#F1FA8C",
],
"bracket-pair-colorizer-2.colorMode": "Consecutive",
"bracket-pair-colorizer-2.forceUniqueOpeningColor": false,
"bracket-pair-colorizer-2.forceIterationColorCycle": false,
"bracket-pair-colorizer-2.showBracketsInGutter": true,
"bracket-pair-colorizer-2.showBracketsInRuler": true,
"bracket-pair-colorizer-2.showVerticalScopeLine": false,
"bracket-pair-colorizer-2.showHorizontalScopeLine": false,
"bracket-pair-colorizer-2.unmatchedScopeColor": "#FF5555",
```

### Code Runner

```json
"code-runner.clearPreviousOutput": true,
"code-runner.ignoreSelection": true,
"code-runner.saveFileBeforeRun": true,
"code-runner.runInTerminal": true,
"code-runner.preserveFocus": false,
"code-runner.executorMap": {
  "python": "python3 -u",
  "typescript": "npx ts-node --files --transpile-only",
},
```

### Meterial Icon Theme

```json
"material-icon-theme.hidesExplorerArrows": true,
"material-icon-theme.folders.theme": "classic",
"material-icon-theme.folders.color": "#6273a6",
```

### Colorize

```json
"colorize.hide_current_line_decorations": false,
"colorize.include": [
  ".tsx",
  ".jsx",
  ".ts",
  ".js"
],
"colorize.languages": [
  "typescriptreact",
  "javascriptreact",
  "javascript",
  "typescript",
  "css",
  "sass",
  "scss",
  "less",
  "pcss",
  "sss",
  "stylus",
  "xml",
  "svg",
  "json",
  "jsonc",
  "yaml"
],
"colorize.colorized_colors": [
  "HEXA",
  "RGB",
  "HSL"
],
"colorize.enable_search_variables": false,
```

### CSpell

```json
"cSpell.enabled": true,
"cSpell.language": "en,pt,pt_BR",
```

**Enjoy!**

## TSLint configuration for Aplaline projects

### Usage

In ```package.json``` add the following to configure eslint:

```
  "devDependencies": {
    "tslint": "^5.10.0",
    "tslint-config-aplaline": "git+https://github.com/aplaline/tslint-config-aplaline#1.0.0",
  }
```

Then create a ```tslint.json``` with the following content:

```
{
  "extends": [
    "tslint-config-aplaline"
  ]
}
```

To get Visual Studio Code to show warnings create ```.vscode/settings.json``` with the following content:

```
{
  "tslint.enable": true
}
```

Additionally it is advised to set the following additional settings in ```.vscode/settings.json```:

```
{
  "editor.lineNumbers": "on",
  "beautify.tabSize": 2,
  "beautify.options": {
    "indent_size": 2
  }
}
```

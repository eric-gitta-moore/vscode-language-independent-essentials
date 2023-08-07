# vscode-language-independent-essentials README


## 包含的扩展

```json5
[
        "Gydunhn.vsc-essentials",
        "ritwickdey.liveserver",
        "donjayamanne.git-extension-pack",
        "amazonwebservices.aws-toolkit-vscode",
        "ms-vscode-remote.vscode-remote-extensionpack",
        "formulahendry.code-runner",
        "ms-azuretools.vscode-docker",
        "wakatime.vscode-wakatime",
        "natizyskunk.sftp",
        "editorconfig.editorconfig",
        "tyriar.sort-lines",
        "uctakeoff.vscode-counter",
        "vscode-icons-team.vscode-icons",
        "vizzuhq.code-viz-stat"
    ]
```

## 建议安装（需要自行安装）

- vim
- Chinese

## 设置替代插件列表

1. Bracket Pair Colorization，【editor.bracketPairColorization.enabled】默认开启
2. Auto Close Tag，【html.autoClosingTags】默认开启
3. Auto Rename Tag，【editor.linkedEditing】需要手动开启
4. Setting Sync，现如今已经自带同步
5. Highlight Matching Tag，【editor.guides.bracketPairs】需要手动开启


## 我的 settings.json
> 尽量简洁为主
```json5
{
    // my settings start
    "git.enableSmartCommit": true,
    "git.autofetch": true,
    "editor.linkedEditing": true,
    "workbench.iconTheme": "vscode-icons",
    "terminal.integrated.fontFamily": "MesloLGS NF",
    "workbench.tree.expandMode": "doubleClick",
    "editor.guides.bracketPairs": "active",
    // plugin settings
    //     prettier-eslint
    "editor.defaultFormatter": "rvest.vs-code-prettier-eslint",
    "editor.formatOnPaste": false, // required 
    "editor.formatOnType": false, // required
    "editor.formatOnSave": true, // optional 
    "editor.formatOnSaveMode": "file", // required to format on save
    "files.autoSave": "onFocusChange", // optional but recommended
    "vs-code-prettier-eslint.prettierLast": false, // set as "true" to run 'prettier' last not first
    //     vim
    "vim.useSystemClipboard": true,
    "vim.handleKeys": {
        "<C-a>": false,
        "<C-x>": false,
        "<C-c>": false,
        "<C-s>": false,
        "<C-k>": false,
        "<C-v>": false,
        "<C-z>": false,
        "<C-n>": false,
    },
    // my settings end
}
```
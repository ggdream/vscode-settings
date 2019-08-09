# vscode-settings
个人vscode定制设置

![vscode](https://ae01.alicdn.com/kf/H0c53949e28cb4885a2a1a38757d00746g.png)



### 基于One Dark Pro编辑器主题和material-icon-theme的图标主题的个人编辑器定制页面。



> settings.json 文件物理存储位置
>
> - Windows: `%APPDATA%\Code\User\settings.json`
> - Mac: `$HOME/Library/Application Support/Code/User/settings.json`
> - Linux: `$HOME/.config/Code/User/settings.json`
>
> 依次点击菜单 `Code > Preferences > Settings` 或 快捷键 `command + ,` 进行设置。


```json
    // 自定义标题栏
    "window.title": "${activeEditorLong}${separator}${rootName}",

    // 保存文件时，去除行尾空格
    "files.trimTrailingWhitespace": true,

    // 隐藏左侧边栏上的 OpenEditors
    "explorer.openEditors.visible": 0,

    // 字号
    "editor.fontSize": 15,
    "editor.fontWeight":  "500",
    "editor.lineHeight": 25,
    "editor.tabSize": 2,

    // 字体
    "editor.fontFamily": "'Fira Code', Source Code Pro, Menlo, Monaco, 'Courier New', monospace",

    // 软件主题配色
    "workbench.iconTheme": "material-icon-theme", // 图标主题
    "workbench.colorTheme": "One Dark Pro", // 颜色主题
    "workbench.colorCustomizations": {
        "[One Dark Pro]": {
            // 编辑区域背景
            "editor.background": "#2E2E2E",
            // 侧边栏
            "sideBar.background": "#2E2E2E",
            "sideBar.foreground": "#999",
            "sideBar.border": "#2E2E2E",
            // 侧边栏列表
            "list.inactiveSelectionBackground": "#32363d",
            "list.inactiveSelectionForeground": "#dfdfdf",
            "list.hoverBackground": "#32363d",
            "list.hoverForeground": "#dfdfdf",
            // peek 窗口
            "peekView.border": "#5b99fc9c",
            // 顶部 tab 栏
            "tab.border": "#2e2e2e",
            "tab.activeBackground": "#2e2e2e",
            "tab.activeForeground": "#cfcfcf",
            "tab.activeBorder": "#5b99fcb9",
            "tab.hoverBackground": "#2e2e2e",
            "tab.hoverBorder": "#5b99fcb9",
            "tab.inactiveForeground": "#8e8e8e",
            // 最左侧工具栏
            "activityBar.background": "#2e2e2e",
            // 状态栏
            "statusBar.background": "#2e2e2e",
            // panel 窗口
            "panelTitle.activeBorder": "#5b99fc5b",
            "panelTitle.activeForeground": "#cfcfcf",
            // 光标
            "editorCursor.foreground": "#84B1ED",
            // 当前行
            "editor.lineHighlightBackground": "#32363d",
            //
            // "editorIndentGuide.activeBackground": "#5b99fc33",
            // 行号栏的当前行
            "editorLineNumber.activeForeground": "#9CA5B4",
            // 行号
            "editorLineNumber.foreground": "#777",
            // 标尺
            "editorRuler.foreground": "#3f3f3f",
            // 快捷提示窗口
            "editorSuggestWidget.highlightForeground": "#84B1ED",
            "editorSuggestWidget.selectedBackground": "#333f5c",
            // 单击一个词时，其它相同单词
            "editor.selectionHighlightBackground": "#ffe7921c",
            "editor.selectionBackground": "#434e61c9",
            // "editor.selectionHighlightBorder": "#90e97259",
            // terminal 中的光标
            "terminalCursor.foreground": "#84B1ED",
            // 侧边栏中一块区域的标题
            "sideBarSectionHeader.background": "#32363d",
            // 区域获取焦点时
            "focusBorder": "#5b99fc36",
        }
    },

    // 快速打开文件时，关闭预览模式，直接打开文件
    "workbench.editor.enablePreviewFromQuickOpen": false,

    // 单击侧边栏打开文件时，关闭预览模式，直接打开文件
    "workbench.editor.enablePreview": false,

    // 导航路径
    "breadcrumbs.enabled": true ,

    // 使用 ctrl 或 command 多选
    "editor.multiCursorModifier": "ctrlCmd",

    // 新打开 vscode 时，编辑器创建新文件
    "workbench.startupEditor": "newUntitledFile",

    // 文件对比窗口，忽略空白字符
    "diffEditor.ignoreTrimWhitespace": true,

    // 编辑器中，快速提示框的位置
    "editor.snippetSuggestions": "top",

    // 每行输入字符长度提示线
    "editor.rulers": [120],

    // 光标宽度
    "editor.cursorWidth": 2,
    "editor.cursorBlinking": "smooth",
    "editor.cursorSmoothCaretAnimation": true,

    // terminal 光标样式
    "terminal.integrated.cursorBlinking": true,
    "terminal.integrated.cursorStyle": "line",

    // 当前行对应的行号栏也高亮显示
    "editor.renderLineHighlight": "all",

    // 右侧的 minimap
    // "editor.minimap.enabled": false, // 隐藏
    "editor.minimap.showSlider": "always", // 一直显示滚动条
    "editor.minimap.renderCharacters": false,
    "editor.minimap.maxColumn": 200,

    // 平滑滚动
    "editor.smoothScrolling": true,

    // 空格显示
    "editor.renderWhitespace": "all",

    // 禁止滚动到文件最后一行后还能继续滚动
    "editor.scrollBeyondLastLine": false,

    // 禁止链接文字可点击，取消下划线
    "editor.links": false,

    // 基于编辑器设置的颜色主题，自定义语法着色
    "editor.tokenColorCustomizations": {
        "[One Dark Pro]": {
            "comments": "#6E7783",
            "keywords": "#F16B6F",
            "variables": "#EFDC05",
            "strings": "#5CAB7D",
            "functions": "#ff7473",
            "numbers": "#ffc952",
        }
    },

    // 禁止提交匿名数据（需要重新启动软件）
    "telemetry.enableTelemetry": false,
    "telemetry.enableCrashReporter": false,

    // 自定义文件关联
    "files.associations": {
        "*.wxss": "css",
        "*.html": "html",
    },

    // 搜索时需要忽略的文件或目录
    "search.exclude": {
        "**/node_modules": true,
        "**/bower_components": true,
        "**/.svn": true,
        "**/.git": true,
    },

    // 忽略工程打开的文件或目录
    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/CVS": true,
        "**/.DS_Store": true,
    },

    // 打开浏览器设置
    "open-in-browser.default": "Google Chrome",

    //--------------------------------------------------
    // 内置插件配置
    //--------------------------------------------------

    // html 中 style 属性里写 css 快速提示
    "[html]": {
        "editor.quickSuggestions": {
            "other": true,
            "comments": false,
            "strings": true,
        },
        "editor.quickSuggestionsDelay": 500,
    },

    // Emmet
    "emmet.triggerExpansionOnTab": true,
    "emmet.includeLanguages": {
        "javascript": "javascriptreact",
    },
    "liveServer.settings.donotShowInfoMsg": true
}
```


## 声明

仅用于学习个人使用，如有侵权请联系删除。E-mail：[lyle.lypm@gmail.com](mailto:lyle.lypm@gmail.com)

## 参与我们

如果有任何想法或需求，可以在 [issue](https://github.com/tickmao/vscode-settings/issues) 中告诉我们，欢迎各种小伙伴踊跃留言。
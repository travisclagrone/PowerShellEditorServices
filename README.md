# PowerShell Editor Services

[![Build Status](https://powershell.visualstudio.com/PowerShellEditorServices/_apis/build/status/PowerShellEditorServices-ci?branchName=master)](https://powershell.visualstudio.com/PowerShellEditorServices/_build/latest?definitionId=50&branchName=master)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/fb9129c327dc4f459ad2fd167d9a574f)](https://app.codacy.com/app/TylerLeonhardt/PowerShellEditorServices?utm_source=github.com&utm_medium=referral&utm_content=PowerShell/PowerShellEditorServices&utm_campaign=Badge_Grade_Dashboard)
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=PowerShell/PowerShellEditorServices)](https://dependabot.com)
[![Discord](https://img.shields.io/discord/180528040881815552.svg?label=%23vscode&logo=discord&logoColor=white)](https://aka.ms/psdiscord)
[![Join the chat at https://gitter.im/PowerShell/PowerShellEditorServices](https://badges.gitter.im/PowerShell/PowerShellEditorServices.svg)](https://gitter.im/PowerShell/PowerShellEditorServices?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

PowerShell Editor Services is a PowerShell module that provides common
functionality needed to enable a consistent and robust PowerShell development
experience in almost any editor or integrated development environment (IDE).

## PowerShell Language Server Protocol clients using PowerShell Editor Services

The functionality in PowerShell Editor Services is already available in the following editor extensions:

- [The VSCode PowerShell extension](https://github.com/PowerShell/vscode-powershell), also available in Azure Data Studio
- [coc-powershell](https://github.com/yatli/coc-powershell), a vim/neovim PowerShell plugin
- [The IntelliJ PowerShell plugin](https://github.com/ant-druha/intellij-powershell)
- [lsp-powershell](https://github.com/kiennq/lsp-powershell), an Emacs PowerShell plugin

## Features

- The Language Service provides common editor features for the PowerShell language:
  - Code navigation actions (find references, go to definition)
  - Statement completions (IntelliSense)
  - Real-time semantic analysis of scripts using PowerShell Script Analyzer
- The Debugging Service simplifies interaction with the PowerShell debugger (breakpoints, variables, call stack, etc)
- The [$psEditor API](http://powershell.github.io/PowerShellEditorServices/guide/extensions.html) enables scripting of the host editor
- A full, terminal-based Integrated Console experience for interactive development and debugging

## Development

### 1. Install PowerShell 6+

Install PowerShell 6+ with [these instructions](https://github.com/PowerShell/PowerShell#get-powershell).

### 3. Clone the GitHub repository:

```
git clone https://github.com/PowerShell/PowerShellEditorServices.git
```

### 4. Install [Invoke-Build](https://github.com/nightroman/Invoke-Build)

```powershell
Install-Module InvokeBuild -Scope CurrentUser
```

Now you're ready to build the code.  You can do so in one of two ways:

### Building the code from PowerShell

```powershell
PS C:\path\to\PowerShellEditorServices> Invoke-Build Build
```

### Building the code from Visual Studio Code

Open the PowerShellEditorServices folder that you cloned locally and press <kbd>Ctrl+Shift+B</kbd>
(or <kbd>Cmd+Shift+B</kbd> on macOS).

## Contributions Welcome!

We would love to incorporate community contributions into this project.  If you would like to
contribute code, documentation, tests, or bug reports, please read our [Contribution Guide](http://powershell.github.io/PowerShellEditorServices/CONTRIBUTING.html) to learn more.

## Maintainers

- [Keith Hill](https://github.com/rkeithhill) - [@r_keith_hill](http://twitter.com/r_keith_hill)
- [Patrick Meinecke](https://github.com/SeeminglyScience) - [@SeeminglyScienc](http://twitter.com/SeeminglyScienc)
- [Tyler Leonhardt](https://github.com/tylerleonhardt) - [@TylerLeonhardt](http://twitter.com/tylerleonhardt)
- [Rob Holt](https://github.com/rjmholt) - no twitter

## License

This project is [licensed under the MIT License](LICENSE).

## [Code of Conduct][conduct-md]

This project has adopted the [Microsoft Open Source Code of Conduct][conduct-code].
For more information see the [Code of Conduct FAQ][conduct-FAQ] or contact [opencode@microsoft.com][conduct-email] with any additional questions or comments.

[conduct-code]: http://opensource.microsoft.com/codeofconduct/
[conduct-FAQ]: http://opensource.microsoft.com/codeofconduct/faq/
[conduct-email]: mailto:opencode@microsoft.com
[conduct-md]: https://github.com/PowerShell/PowerShellEditorServices/blob/master/CODE_OF_CONDUCT.md

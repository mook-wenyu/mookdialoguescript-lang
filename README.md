# MookDialogueScript 对话脚本语言
# MookDialogueScript Dialogue Script Language

[中文](#chinese) | [English](#english)

<a name="chinese"></a>
## 中文说明

这个 VSCode 扩展为 MookDialogueScript 对话脚本语言提供语法高亮和编辑辅助功能。MookDialogueScript 是一个专门用于编写游戏对话和剧情的脚本语言，支持分支对话、条件判断、变量系统等功能。

对话脚本系统的完整实现请参考：[MookDialogueScriptFromUnity](https://github.com/mook-wenyu/MookDialogueScriptFromUnity)

### 主要特性

- **完整的语法高亮支持**
  - 节点定义：`--- 节点名`
  - 节点结束标记：`===`
  - 元数据标记：`[key: value]` 或 `【key：value】`（节点定义后的一行或连续多行）
    - 特殊元数据：`[title: 标题]`（使用特殊高亮）
  - 条件语句（`if`、`elif`、`else`、`endif`）
  - 系统命令（`var`、`set`、`call`、`wait`、`jump` 等）
  - 变量系统（`$变量名`）
  - 多种对话形式
  - 选项系统
  - 注释支持（`//` 开头，必须独立一行）

- **智能代码片段**
  - 快速插入常用语法结构
  - 支持中英文符号
  - 自动补全和提示

- **便捷的编辑功能**
  - 自动缩进
  - 代码折叠
  - 智能括号匹配

### 安装和使用

1. 在 VSCode 扩展市场中搜索 "MookDialogueScript" 并安装
2. 安装完成后，创建一个以 `.mds` 为扩展名的文件
3. 开始编写对话脚本，享受语法高亮和代码片段支持

### 代码片段速查表

| 代码片段 | 描述 | 示例 |
|---------|------|------|
| `node` / `节点` | 创建节点 | `--- 节点名` ... `===` |
| `metadata` / `元数据` | 添加元数据 | `[key: value]` |
| `choice` / `选项` | 添加选项 | `-> 选项文本` |
| `if` | 条件分支 | `if $条件` |
| `character` / `角色` | 角色对话 | `角色名: 对话` |


<a name="english"></a>
## English

This VSCode extension provides syntax highlighting and editing support for MookDialogueScript, a scripting language designed for writing game dialogues and narratives.

For the complete dialogue script system implementation, please refer to: [MookDialogueScriptFromUnity](https://github.com/mook-wenyu/MookDialogueScriptFromUnity)

### Key Features

- **Full Syntax Highlighting**
  - Node definitions: `--- nodename`
  - Node ending marker: `===`
  - Metadata markers: `[key: value]` or `【key：value】` (one or more lines after node definition)
    - Special metadata: `[title: title]` (with special highlighting)
  - Conditional statements (`if`, `elif`, `else`, `endif`)
  - System commands (`var`, `set`, `call`, `wait`, `jump`, etc.)
  - Variable system (`$varname`)
  - Multiple dialogue formats
  - Choice system
  - Comment support (`//` at the beginning, must be on its own line)

- **Smart Snippets**
  - Quick insertion of common syntax structures
  - Support for both English and Chinese punctuation
  - Auto-completion and hints

- **Convenient Editing Features**
  - Auto-indentation
  - Code folding
  - Smart bracket matching

### Installation and Usage

1. Search for "MookDialogueScript" in the VSCode extension marketplace and install it
2. After installation, create a file with the `.mds` extension
3. Start writing dialogue scripts with syntax highlighting and snippet support

### Snippet Quick Reference

| Snippet | Description | Example |
|---------|-------------|---------|
| `node` | Create node | `--- nodename` ... `===` |
| `metadata` | Add metadata | `[key: value]` |
| `choice` | Add choice | `-> choice text` |
| `if` | Condition branch | `if $condition` |
| `character` | Character dialogue | `name: dialogue` |


## License

Apache License 2.0 - see the [LICENSE](LICENSE.txt) file for details.

# MookDialogueScript 对话脚本语言
# MookDialogueScript Dialogue Script Language

[中文](#chinese) | [English](#english)

<a name="chinese"></a>
## 中文说明

这个 VSCode 扩展为 MookDialogueScript 对话脚本语言提供语法高亮和编辑辅助功能。MookDialogueScript 是一个专门用于编写游戏对话和剧情的脚本语言，支持分支对话、条件判断、变量系统等功能。

### 主要特性

- **完整的语法高亮支持**
  - 节点定义（`::节点名` 或 `：：节点名`）
  - 条件语句（`if`、`elif`、`else`、`endif`）
  - 系统命令（`var`、`set`、`call`、`wait`、`jump` 等）
  - 变量系统（`$变量名`）
  - 多种对话形式
  - 选项系统
  - 注释支持

- **智能代码片段**
  - 快速插入常用语法结构
  - 支持中英文符号
  - 自动补全和提示

- **便捷的编辑功能**
  - 自动缩进
  - 代码折叠
  - 智能括号匹配

### 快速开始

1. 安装扩展后，创建一个以 `.mds` 为扩展名的文件
2. 使用以下基本语法开始编写对话脚本：

```mds
:: 开始
    这是一段旁白文本。
    
    小明: 你好，这是一段对话。
    小红[开心]: 你也好！
    
    -> 继续聊天
        小明: 今天天气真好！
        => 天气话题
        
    -> 结束对话 [if $时间 > 18]
        小明: 时间不早了，明天见！
        => 结束

:: 天气话题
    if $下雨 == true
        小红: 可是外面在下雨呢。
    else
        小红: 是啊，阳光正好！
    endif
```

### 代码片段速查表

| 代码片段 | 描述 | 示例 |
|---------|------|------|
| `node` / `节点` | 创建新节点 | `:: 节点名` |
| `choice` / `选项` | 添加选项 | `-> 选项文本` |
| `if` | 条件分支 | `if $条件` |
| `character` / `角色` | 角色对话 | `角色名: 对话` |


<a name="english"></a>
## English

This VSCode extension provides syntax highlighting and editing support for MookDialogueScript, a scripting language designed for writing game dialogues and narratives.

### Key Features

- **Full Syntax Highlighting**
  - Node definitions (`::nodename`)
  - Conditional statements (`if`, `elif`, `else`, `endif`)
  - System commands (`var`, `set`, `call`, `wait`, `jump`, etc.)
  - Variable system (`$varname`)
  - Multiple dialogue formats
  - Choice system
  - Comment support

- **Smart Snippets**
  - Quick insertion of common syntax structures
  - Support for both English and Chinese punctuation
  - Auto-completion and hints

- **Convenient Editing Features**
  - Auto-indentation
  - Code folding
  - Smart bracket matching

### Quick Start

1. After installing the extension, create a file with the `.mds` extension
2. Start writing dialogue scripts using the following basic syntax:

```mds
:: start
    This is a narration text.
    
    John: Hello, this is a dialogue.
    Mary[happy]: Hi there!
    
    -> Continue chatting
        John: The weather is nice today!
        => weather_topic
        
    -> End conversation [if $time > 18]
        John: It's getting late, see you tomorrow!
        => end

:: weather_topic
    if $raining == true
        Mary: But it's raining outside.
    else
        Mary: Yes, the sunshine is perfect!
    endif
```

### Snippet Quick Reference

| Snippet | Description | Example |
|---------|-------------|---------|
| `node` | Create new node | `:: nodename` |
| `choice` | Add choice | `-> choice text` |
| `if` | Condition branch | `if $condition` |
| `character` | Character dialogue | `name: dialogue` |


## License

Apache License 2.0 - see the [LICENSE](LICENSE.txt) file for details.

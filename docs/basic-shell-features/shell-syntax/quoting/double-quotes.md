在双引号 `"` 中的任何字符都代表它本身的字面含义，除了『`$`』、『`'`』、『`\`』，若启用了历史命令扩展，`!` 也包括在内。当 Shell 处于 POSIX 模式时,就算打开了历史命令扩展，`!` 在双引号中也没有特殊含义。`$` 与 `'` 在双引号中依旧有特殊含义。在双引号中，如果反斜线后面跟着 `$`、`'`、`"`、`\` 或 `newline`，它才有特殊含义，这些反斜线会被去掉。没有特殊含义字符前面的反斜线不会受到影响。在一对双引号中，可以通过使用反斜线嵌入双引号。在启用历史命令扩展的情况下，如过 `!` 没有转义，那么 `!` 打头的命令会被扩展。`!` 前面的反斜线不会被去掉。

特殊参数 `*` 和 `@` 在双引号中也有特殊含义。
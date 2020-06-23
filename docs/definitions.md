# 概念

这些概念将会贯穿整本手册。

- `POSIX`   一系列基于 Unix 的开放系统标准。`Bash` 主要跟 *POSIX 1003.1* 标准中的 *Shell and Utilities* 部分有关系。
- `blank`   一个空格或者制表符。
- `builtin`   由 shell 内部实现的命令，而非存储在文件系统中的某个可执行程序。
- `control operator`   一个能执行控制函数的标记。它可能是 `newline`，或者下面这些中的任意一个：`||`、`&&`、`&`、`;`、`;;`、`;&`、`;;&`、`|`、`|&`、`(` 或 `)`
- `exit status`   返回给调用命令的程序的一个值。这个值被严格限制在 8 个比特（bit），所以它的最大值是 255。
- `field`   任意 shell 扩展之后的结果，是一个字段。在扩展完成后，执行一个命令，扩展之后的字段作为命令名或者参数使用。
- `filename`   用于标识一个文件的字符串。
- `job`   一组由管道组成的进程集，以及任何衍生的子进程，都属于同一个进程组。
- `job control`   一种机制，用户可以选择性停止（暂停）或者重启（恢复）进程的执行。
- `metacharacter`   没有被引号包裹时，用来分隔单词的字符。一个元字符可以是一个 `space`、`tab`，`newline` 或者以下任意一个：`|`、`&`、`;`、`(`、`)` 或 `<`、`>`。
- `name`   一个仅由字母、数字和下划线，并且以字母或者下划线打头的单词。`names` 被用作 shell 变量和函数名。也可以叫 `identifier`。
- `operator`   一个**控制操作符**或者**重定向操作符**。3.6 章节会列 重定向操作符。它们包含至少一个未被引号包裹的 `metacharacter`。
- `process group`  一组相关进程集合，它们共享同一个进程组 ID。
- `process group id`   在生命周期内，代表一个进程组的唯一标识。
- `reserved word`   对 shell 来说有特殊含义的词汇。大多数保留词用在 shell 流控结构的开头，比如 `for` 与 `while`。
- `return status`   `exit status` 的同义词。
- `signal`   通过这种机制，内核可以通过系统事件对进程发出提醒。
- `special builtin`   被 `POSIX` 标准划分为特殊的 shell  内置命令。
- `token`   被 shell 看作一个单元的字符串。要么是 `word`，要么是 `operator`。
- `word`   被 shell 当一个单元处理的字符串。`words` 不包括未引用的 `metacharacters`。
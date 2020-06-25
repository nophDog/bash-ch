美元符（『`$`』）后面的双引号字符串会被翻译成当前区域的文字。如果当前区域设置为 `C` 或者 `POSIX`，那么美元符会被忽略。

有些系统使用由 `LC_MESSAGE` shell 变量选择的消息目录。还有些会根据 `TEXTDOMAIN` shell 变量生成消息目录的名字，或许会加上一个后缀 `.mo`。如果使用 `TEXTDOMAIN` 变量，你需要在把它设置成消息目录文件的位置。还有些人会这样混合使用这两个变量：`TEXTDOMAIN/LC_MESSAGES/LC_MESSAGES/TEXTDOMAIN.mo`。
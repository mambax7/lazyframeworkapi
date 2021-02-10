# 2-9 Get the language family get\_lang\($type\)

### 2-9 Get language get\_lang\($type\)

```text
get_lang($type):array
```

Generally speaking, developers don't need to use it. This method will be used in xoops\_version.php to get the language of the module.

1. `$type`:RequiredLanguage family type, which can be `mi`\(the language family of the profile\), `ma`\(the language family of the background\), `md`\(the language family of the foreground\), `mb`\(the language family of the block\)


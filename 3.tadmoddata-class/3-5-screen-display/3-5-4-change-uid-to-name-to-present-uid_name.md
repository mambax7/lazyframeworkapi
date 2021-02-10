# 3-5-4 Change uid to name to present uid\_name\(\)

#### 3-5-4 Change uid to name to present uid\_name\(\)

```text
uid_name($col_name = 'uid', $type = 1):object
```

Converting the user ID to the real name will automatically apply to each method, and automatically generate a new field of "field name\_name", such as "uid\_name" can also be used in the template label.

1. `$col_name`: \(The default is `uid`\) the field name of the user ID. If the field of the user ID happens to be called `uid`, it doesn’t matter if you don’t need to fill it in.
2. `$type`: \(Default is  `1`\) that is to obtain the real name, if  `0`yes, it is to obtain the account.


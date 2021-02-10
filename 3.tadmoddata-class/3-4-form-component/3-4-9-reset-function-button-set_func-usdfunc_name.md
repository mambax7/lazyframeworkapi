# 3-4-9 Reset function button set\_func\($func\_name\)

#### 3-4-9 Reset function button set\_func\($func\_name\)

```text
set_func($func_name, $to = false):object
```

You can reset the default function link button, you can hide it, or you can modify the link position again

1. `$func_name`: RequiredMethod button to be reset \(i.e. `create`, `edit`, `show`, `update`, `store`, `destroy`, `index`\) as a
2. `$to`: \(Default `false`\) you can specify where the button is to be connected. If it is set, `false`the button is not used.


# 2-4 New front-end menu add\_menu\($title, $value\)



### 2-4 New front-end menu add\_menu\($title, $value\)

```text
add_menu($title, $value, $only_adm = false):object
```

The default package is in the function.php of the blank module, which is used to set the front-end module menu. If it is not necessary, setting one group will generate one option, and multiple groups can be used.

1. `$title`: Required Option name
2. `$value`: Required Destination URL
3. `$only_adm`: \(Default value `false`\) whether only the administrator can see


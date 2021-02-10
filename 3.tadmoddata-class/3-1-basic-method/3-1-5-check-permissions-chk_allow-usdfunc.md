# 3-1-5 check permissions chk\_allow\($func\)

#### 3-1-5 Check permissions chk\_allow\($func\)

```text
chk_allow($func, $redirect = ''):bool
```

You can check permissions for a certain function, if you don’t have permission, you can specify where to go

1. `$func`: Required To check the permissions of the method \(i.e. `create`, `edit`, `show`, `update`, `store`, `destroy`, `index`\) as a
2. `$redirect`: Turning position, if not filled in, it will return to the original page by default


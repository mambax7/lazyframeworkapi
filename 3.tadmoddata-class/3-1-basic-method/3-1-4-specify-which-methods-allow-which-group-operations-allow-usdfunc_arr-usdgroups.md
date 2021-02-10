# 3-1-4 specify which methods allow which group operations allow\($func\_arr, $groups\)

#### 3-1-4 specify which methods allow which group operations allow\($func\_arr, $groups\)

```text
allow($func_arr = [], $groups = []):object
```

This is used to set which methods on this page are only allowed for those groups. At present, only [the seven built-in methods](https://campus-xoops.tn.edu.tw/modules/tad_book3/page.php?tbsn=48&tbdsn=1604) are open . In the future, it should be possible to specify a homemade method...

1. `$func_arr`:RequiredTo allow the process \(i.e. `create`, `edit`, `show`, `update`, `store`, `destroy`, `index`\) array
2. `$groups`:RequiredGroup number array, `1`for administrators, `2`members, and `3`visitors. If the website has a customized group \(such as school staff, students, etc.\) for the remaining numbers, check the group from the background "group" What is the group number.


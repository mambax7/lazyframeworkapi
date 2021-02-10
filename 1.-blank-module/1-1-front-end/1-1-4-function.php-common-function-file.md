# 1-1-4 function.php common function file

```text
<?php
use XoopsModules\Tadtools\TadMod;
$TadMod = new TadMod(basename(__DIR__));
// $TadMod->add_menu('前台選項', 'index.php?op=create', true);
```

Copy

The common function file refers to the functions that will be used in the front and back end and can be written in this file.

The menu at the front desk is also set in this file \(the comment section\). For `add_menu()`details, please refer to: [https://campus-xoops.tn.edu.tw/modules/tad\_book3/page.php?tbsn=48&tbdsn=1641](https://campus-xoops.tn.edu.tw/modules/tad_book3/page.php?tbsn=48&tbdsn=1641)


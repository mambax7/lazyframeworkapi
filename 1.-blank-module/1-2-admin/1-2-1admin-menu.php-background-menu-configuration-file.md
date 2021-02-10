# 1-2-1admin/menu.php background menu configuration file

```text
<?php
use XoopsModules\Tadtools\TadMod;
$TadMod = new TadMod(basename(__DIR__));
$TadMod->add_adm_menu('Module management', 'admin/main.php', 'images/admin/button.png');
$adminmenu = $TadMod->get_adm_menu();
```

Copy

We are here to use the `add_adm_menu()`setting background page menu

Do not move the rest

`add_adm_menu()`Please refer to: [https://campus-xoops.tn.edu.tw/modules/tad\_book3/page.php?tbdsn=1643](https://campus-xoops.tn.edu.tw/modules/tad_book3/page.php?tbdsn=1643)


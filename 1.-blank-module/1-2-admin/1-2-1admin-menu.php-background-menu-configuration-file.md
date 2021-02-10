# 1-2-1admin/menu.php background menu configuration file

```text
<?php
use XoopsModules\Tadtools\TadMod;
$TadMod = new TadMod(basename(__DIR__));
$TadMod->add_adm_menu('Module management', 'admin/main.php', 'images/admin/button.png');
$adminmenu = $TadMod->get_adm_menu();
```

We are here to use the `add_adm_menu()`setting background page menu

Do not move the rest

`add_adm_menu()`Please refer to: [API Tutorial](https://xoops.gitbook.io/jill-lazy-framework-api/2.tadmod-class/untitled/2-6-add-background-menu-add_adm_menu-usdtitle-usdvalue)


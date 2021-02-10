# 1-1-5 footer.php front page footer file

```text
<?php
use XoopsModules\Tadtools\Utility;

if (empty($op)) {
    $op = 'index';
}
if (empty($op_prfix)) {
    $op_prfix = substr(basename($_SERVER['PHP_SELF']), 0, -4);
}
$TadMod->get_menu('toolbar');
$xoopsTpl->assign('now_op', "{$op_prfix}_{$op}");
$xoopsTpl->assign('xoopsModuleConfig', $xoopsModuleConfig);

$xoTheme->addStylesheet(XOOPS_URL . '/modules/' . basename(__DIR__) . '/css/module.css');
$xoTheme->addStylesheet(XOOPS_URL . '/modules/tadtools/css/my-input.css');
include_once XOOPS_ROOT_PATH . '/footer.php';
```

Copy

Every file on the front page needs to include this footer file at the end

This file is used to set the default actions, the name of the template to be used, generate toolbars, and import various appearance style files, etc.

Generally speaking, developers do not need to move to this file.

tadtools&gt;=3.39 Add $xoopsTpl-&gt;assign\('xoopsModuleConfig', $xoopsModuleConfig\);


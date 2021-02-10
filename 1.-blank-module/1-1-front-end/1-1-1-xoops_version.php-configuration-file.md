# 1-1-1 xoops\_version.php configuration file

```text
<?php
use XoopsModules\Tadtools\TadMod;
$TadMod = new TadMod(basename(__DIR__));

// $TadMod->setup('Module name', '1.0', '2020/05/31', 'tad0616@gmail.com', 'Tad');
// $TadMod->add_config('show_num', 'Preference title', '', 'textbox', 'int', 20);
// $TadMod->add_blocks('data_list', 'block title', '', ['display data number' => 10]);

$lang = $TadMod->get_lang('mi');
foreach ($lang as $const_arr) {
    foreach ($const_arr as $const => $value) {
        define($const, $value);
    }
}
$modversion = $TadMod->xoops_version();
```

Copy

The most important configuration file of the XOOPS module, only this file is considered a module.

It is used to set basic information such as module name and version. It is also necessary to set whether to use before, background, template, database and other settings, as well as whether there are blocks, preferences and other information.

In the lazy frame, the parts that need to be set are only the three lines of comments, and the rest of the frame is handled secretly.

`setup()`Please refer to: [https://campus-xoops.tn.edu.tw/modules/tad\_book3/page.php?tbsn=48&tbdsn=1638](https://campus-xoops.tn.edu.tw/modules/tad_book3/page.php?tbsn=48&tbdsn=1638)  
`add_config()` Please refer to: [https://campus-xoops.tn.edu.tw/modules/tad\_book3 /page.php?tbsn=48&tbdsn=1639](https://campus-xoops.tn.edu.tw/modules/tad_book3/page.php?tbsn=48&tbdsn=1639)  
`add_blocks()` Please refer to: [https://campus-xoops.tn.edu.tw/modules/tad\_book3/page.php?tbsn=48&tbdsn=1640](https://campus-xoops.tn.edu.tw/modules/tad_book3/page.php?tbsn=48&tbdsn=1640)


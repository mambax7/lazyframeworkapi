# 1-1-3 header.php Front page header file

```text
<?php
use Xmf\Request;
use XoopsModules\Tadtools\TadUpFiles;

//Load XOOPS mainfile (required)
include_once "../../mainfile.php";
include_once 'preloads/autoloader.php';
include_once "function.php";

$xoopsOption['template_main'] = basename(__DIR__) . '_index.tpl';
include_once XOOPS_ROOT_PATH . "/header.php";

$op = Request::getString('op');
$self = Request::getString('PHP_SELF', '', 'SERVER');
$from = Request::getString('HTTP_REFERER', '', 'SERVER');
$files_sn = Request::getInt('files_sn');

//Download file
if ($op == 'tufdl') {
    $TadUpFiles = new TadUpFiles(basename(__DIR__));
    $TadUpFiles->add_file_counter($files_sn);
    exit;
}
```

Copy

The front-end function page file needs to import this file

This file will load all kinds of things and object types that the XOOPS module needs to load

And will set some variables that will be used on the module page


# 1-2-2admin/main.php background page

```text
<?php
use XoopsModules\Tadtools\TadModData;
use XoopsModules\Tadtools\Utility;
require_once "header.php";

$Model = new TadModData('Model Datatable');
$clean = $Model->clean();

switch ($op) {
    case "create":
        $Model->create();
        break;

    case "edit":
        $Model->edit($clean['primary key']);
        break;

    case "show":
        $Model->show($clean['primary key']);
        break;

    case "update":
        $Model->update($clean['primary key']);
        header("location:{$self}");
        exit;

    case "store":
        $Model->store();
        header("location:{$self}");
        exit;

    case "destroy":
        $Model->destroy($clean['primary key']);
        header("location:{$self}");
        exit;

    default:
        $Model->index();
        break;
}
require_once "footer.php";
```

Copy

Basically, the basic content of all pages in the background is like this \(only the file name is different\)

In fact, the content is the same as the front page, so it is convenient to move the function from the background to the foreground in the future \(just pay attention to the permissions\)

`switch()` Seven basic actions \(almost the concept of routing\) have been set in, of course, they can be increased or decreased according to the function of the page.

`Module Datatable`, Is the name of the datatable that this page needs to use.

`primary key` Refers to the data table `primary key`

You can use more than one on the same page `模型資料表`, and the entity names \(such as `$Model`:\) need to be different to avoid mixing them.


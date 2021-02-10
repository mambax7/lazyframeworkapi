# 1-1-2 index.php front page

```text
<?php
use XoopsModules\Tadtools\TadModData;
use XoopsModules\Tadtools\Utility;
require_once "header.php";

$Model = new TadModData('模型資料表');
$clean = $Model->clean();

switch ($op) {
    case "create":
        $Model->create();
        break;

    case "edit":
        $Model->edit($clean['主鍵']);
        break;

    case "show":
        $Model->show($clean['主鍵']);
        break;

    case "update":
        $Model->update($clean['主鍵']);
        header("location:{$self}");
        exit;

    case "store":
        $Model->store();
        header("location:{$self}");
        exit;

    case "destroy":
        $Model->destroy($clean['主鍵']);
        header("location:{$self}");
        exit;

    default:
        $Model->index();
        break;
}
require_once "footer.php";
```

Copy

Basically, the basic content of all pages in the front desk is like this \(only the file name is different\)

`switch()` Seven basic actions \(almost the concept of routing\) have been set in, of course, they can be increased or decreased according to the function of the page.

`模型資料表`, Is the name of the data table that this page needs to use.

`主鍵`Refers to the data table `primary key`

You can use more than one on the same page `模型資料表`, and the entity names \(such as `$Model`:\) need to be different to avoid mixing them.


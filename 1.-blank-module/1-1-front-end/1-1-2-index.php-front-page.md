# 1-1-2 index.php front page

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
        $Model->edit($clean['Primary key']);
        break;

    case "show":
        $Model->show($clean['Primary key']);
        break;

    case "update":
        $Model->update($clean['Primary key']);
        header("location:{$self}");
        exit;

    case "store":
        $Model->store();
        header("location:{$self}");
        exit;

    case "destroy":
        $Model->destroy($clean['Primary key']);
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

`Model datatable`, Is the name of the data table that this page needs to use.

`Primary key` Refers to the data table `primary key`

You can use more than one `Model datatable` on the same page , but the entity names \(such as `$Model`\) need to be different to avoid mixing them.


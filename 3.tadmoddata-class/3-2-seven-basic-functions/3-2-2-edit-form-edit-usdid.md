# 3-2-2 Edit form edit\($id\)

#### 3-2-2 Edit form edit\($id\)

```text
edit($id, $action = '', $id_name = 'myForm', $def_val = []):string
```

According to the data table field of the model, the form for modification is automatically generated, and the original value is obtained by using the entered primary key for modification. Like create\(\), in addition to returning the complete form content, it will also be automatically applied **&lt;{$ Table name\_form}&gt;** to the template

1. `$id`:Required The number of the data to be modified, usually the primary key \( `primary key`\)
2. `$action`: The location where the form is sent, if not filled in, it will be sent to its own page
3. `$id_name`: \(Default is `myForm`\) the id attribute of the form
4. `$def_val`:tadtools &gt;= 2.39 Mandatory set the default value, the array is `['field' => 'new value']`


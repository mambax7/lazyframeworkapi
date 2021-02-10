# 3-2-3 show single content show\($id\)

#### 3-2-3 show single content show\($id\)

```text
show($id, $where = []):string
```

According to the model data table field, the content of a single page is automatically generated. In addition to returning the complete page content, it will also automatically apply **&lt;{$table name\_show}&gt;** to the template. In addition, all data arrays The template label **&lt;{$table name}&gt;** can be used to display the value of a certain field with **&lt;{$table name. Column name}&gt;**

1. `$id`:RequiredThe data number to be displayed, usually the primary key \( `primary key`\)
2. `$where`: Filter conditions, array format, in order to set multiple sets of filter conditions, currently only supports `and`


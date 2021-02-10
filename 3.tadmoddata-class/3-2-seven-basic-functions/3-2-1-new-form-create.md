# 3-2-1 New form create\(\)



#### 3-2-1 New form create\(\)

```text
create($def_val = [], $action = '', $id_name = 'myForm'):string
```

According to the data table field of the model, a new form is automatically generated. In addition to returning the complete form content, it will also automatically apply **&lt;{$table name\_form}&gt;** to the template

1. `$def_val`: The form default value array, you can specify the default value of the form field
2. `$action`: The location where the form is sent, if not filled in, it will be sent to its own page
3. `$id_name`: \(Default is `myForm`\) the id attribute of the form


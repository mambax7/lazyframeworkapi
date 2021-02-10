# 3-5-6 Fields not displayed disable\($col\_name\)

#### 3-5-6 Fields that are not displayed disable\($col\_name\)

```text
disable($col_name , $where = ['index'], $exception_group = []):object
```

Some fields do not need to be displayed, we can use this method to close some fields. Note that it is just set to not display, but the data still exists, and the template label alone can still be used.

1. `$col_name` :RequiredSet the field name not to be displayed
   * The default is a string, that is, "field name".
   * tadtools&gt;=3.39 It supports array writing.
2. `$where`: \(Default `['index']`\) refers to which functions do not appear, array type, currently there are three values ​​that can be set: `index`\(list\), `show`\(single data\), `create`\(edit form\)
   * If it is applied to the `create`\(editing form\), it means that the field is not used at all, and the field will be a null value instead of hiding the field.
3. `$exception_group`: Exception group, also an array, fill in the group number array, any group in this array, the field will not be hidden


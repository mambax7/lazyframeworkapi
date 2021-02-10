# 3-4-2 single selection box use\_radio\($col\_name, $options = \[\]\)

#### 3-4-2 Single selection box use\_radio\($col\_name, $options = \[\]\)

```text
use_radio($col_name, $options = [], $def_val = null, $validate = ''):string
```

Use a circular radio button to display the specified field

1. `$col_name`:RequiredIt refers to which field in the current form should be replaced with a circular radio button. Please fill in the field name.
2. `$options`:RequiredOption array, the array index is the option value, and the array value is the option presentation text.
3. `$def_val`: You can set the default value, its value should be `$options`in an array index \(ie an option value meaning\)
4. `$validate`: Apply validation rules. If only ture is entered, it means required. For more detailed verification, please refer to [https://github.com/posabsolute/jQuery-Validation-Engine\#validators](https://github.com/posabsolute/jQuery-Validation-Engine#validators) . For example, in addition to required fields, verify whether It is an Email format and can be filled with complete verification rules, such as:`validate[required,custom[email]]`


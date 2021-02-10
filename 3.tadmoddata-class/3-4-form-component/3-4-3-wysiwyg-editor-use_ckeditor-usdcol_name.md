# 3-4-3 WYSIWYG editor use\_ckeditor\($col\_name\)

#### 3-4-3 WYSIWYG editor use\_ckeditor\($col\_name\)

```text
use_ckeditor($col_name, $options = [], $def_val = null):string
```

Use the CKEditor WYSIWYG editor to render the specified fields

1. `$col_name`:RequiredIt refers to which field in the current form should be replaced by a WYSIWYG editor. Please fill in the field name.
2. `$options`:RequiredWYSIWYG editor settings, such as `['setHeight' => 150, 'setToolbarSet' => 'tadSimple']`.
   * `setHeight`Set the height of the editing area, such as 150
   * `setToolbarSet`Toolbar settings \(the amount of the difference function\), the available values are `my`\(the default and most powerful\), `myBasic`, `mySimple`,`tadSimple`
3. `$def_val`: Can set the default value


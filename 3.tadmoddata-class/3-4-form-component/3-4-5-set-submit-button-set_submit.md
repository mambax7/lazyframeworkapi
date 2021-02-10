# 3-4-5 set submit button set\_submit\(\)

#### 3-4-5 Set submit button set\_submit\(\)

```text
set_submit($name = 'op', $value = '', $label = '', $icon = '', $attr_arr = ['class' => 'btn btn-primary']):string
```

Reset send button

1. `$name`:\( default `op`\) set the eject button `name`attribute value
2. `$value`: Set the  `value`attribute value of the send button
3. `$label`: Set the text on the send button
4. `$icon`: Set the [font-awesome icon](https://fontawesome.com/v4.7.0/icons/) on the send button , such as:, `fa-plus`if it is empty, it means no icon
5. `$attr_arr`: \(The default is `['class' => 'btn btn-primary']`, that is , it will be added by default `class="btn btn-primary"`\) You can set other attribute arrays of the submit button


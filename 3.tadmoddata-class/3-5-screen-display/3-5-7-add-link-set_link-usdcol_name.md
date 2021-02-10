# 3-5-7 add link set\_link\($col\_name\)

#### 3-5-7 add link set\_link\($col\_name\)

```text
set_link($col_name, $to = '', $parameter = [], $target = '_self'):object
```

You can add a link to a field

1. `$col_name`:RequiredThe name of the field to be linked
2. `$to`: Link location, if not filled in, it will link to your own page
3. `$parameter`: The parameter array will be automatically connected behind the link
   * If it is a custom parameter, the "array index" is the parameter name, and the "array value" is the parameter value, for example:`['op' => 'show']`
   * If you need to automatically obtain the parameter value, just fill in a field name, for example:, `['action_id']`so when the content is generated, `action_id`the value will be automatically captured and brought into
4. `$target`: \(Default `_self`\) the opening position of the link. If you want to open a new window, please use`_blank`


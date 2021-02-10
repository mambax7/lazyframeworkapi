# 3-5-8 Add custom button add\_button\($title\)

#### 3-5-8 Add custom button add\_button\($title\)

```text
add_button($title, $to = '', $parameter = [], $attr = [], $where = [], $allow = [], $deny = []):object
```

Create link button

1. `$title`:RequiredButton text
2. `$to`: Connect to that file. If you leave it blank, it is the current file, such as:`index.php`
3. `$parameter`: Parameters to be brought after the file \(the same usage as adding a link\), array type
   * If it is a custom parameter, the "array index" is the parameter name, and the "array value" is the parameter value, for example:`'op' => 'create'`
   * If you need to automatically obtain the parameter value, just fill in a field name, for example:, `'action_id'`so when the content is generated, `action_id`the value will be automatically captured and brought into
4. `$attr`: HTML attribute array of buttons, for example, to add the appearance of buttons, we can use `['class' => 'btn btn-sm btn-primary']`to set the
5. `$where`: Set where to add this button to the `index`list, `show`apply to a single page, `create`or apply to the form, for example: `['index', 'show']`add a button to the list and single page.
6. `$allow`: You can see the group array of this button, for example: `[1,2]`to set administrators and members to see, blank means no limit
7. `$deny`: Can not see the group array of this button, for example: `[3]`to set that only visitors can not see, blank means no restriction


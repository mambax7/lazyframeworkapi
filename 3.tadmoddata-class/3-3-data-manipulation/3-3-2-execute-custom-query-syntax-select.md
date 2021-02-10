# 3-3-2 execute custom query syntax select\(\)



#### 3-3-2 Execute custom query syntax select\(\)

```text
select($select_col = '*', $where_item = [], $single = false, $key = '', $tpl_tag = ''):array
```

tadtools &gt;= 3.39More flexible query syntax than find\(\), you can customize the grab field, or customize the SQL syntax, it will return the array, or automatically send the label to the template.

1. `$select_col`: \(Default `*`\) the field to be searched
   * Can be a string \(more flexible or free\), such as:, ``'`id`, `title`, `name`'``or``'`title`, sum(`amount`)'``
   * It can also be an array \(more concise\), such as:, `['id', 'title', 'name']`or`['title', 'sum'=>'amount']`
2. `$where_item`: Where filter array or string
   * It can be a string \(more flexible or free, you need to add it yourself `where`\), such as:```where enable`='1' and date > '2020-06-30' gorup by `title` order by `sort```
   * May be an array of \(relatively compact, but only support `and`and `=`\), such as: `['enable'=>1, date => '2020-06-30']`, ``where `enable`='1' and date='2020-06-30'``becomes: .
   * If a keyword is encountered `uid`and its value is not set, `['uid']`the default will capture the `uid編號`value of the current login, which ``where `uid`='1'``means : meaning \(assuming the current login ID is 1\)
3. `$single`: \(Default is `false`\) whether to use single pen mode.
   * In general are multi-mode pen data, will return as: `$arr[0][id]`, `$arr[0][title]`, `$arr[1][id]`, `$arr[1][title]`like this array.
   * If single mode, it returns only a sum, when determining the sum of your information only, can be set , `true`would pass would be more simple `$arr[id]`,`$arr[title]`
4. `$key`: Set the name of the field used as the index of the result array \(only valid in multi-stroke mode\)
   * If not set, it is the default increment from 0
   * If it is set, please set the field name, for example:, `id`so, the change will use the `id`number as the array index \(the execution statement needs to include the value of the field\)
5. `$tpl_tag`：The name of the label to be sent to the template
   * Such as: `data`, then there are `<{$data.0.id}>`, `<{$data.0.title}>`, `<{$data.1.id}>`, `<{$data.1.title}>`and other labels can be used, if the `single`pattern is `<{$data.id}>`, `<{$data.title}>`and other labels available
   * If it is not set, there will be no template label and only the result array will be returned.


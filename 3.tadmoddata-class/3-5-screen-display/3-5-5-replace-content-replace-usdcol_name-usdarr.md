# 3-5-5 Replace content replace\($col\_name, $arr\)

#### 3-5-5 Replace content replace\($col\_name, $arr\)

```text
replace($col_name, $arr = [], $callback = [], $exception_group = []):object
```

Replace the database value of the specified field with another value to present it, for example, change 0 to "off" and 1 to "on"

1. `$col_name`:RequiredIt refers to the display value of which field to replace.
2. `$arr`: Display value array, the array index is the display value, and the array value is the text to be displayed. The value of this array can be made, with or `get_arr()`acquires array.
3. `$callback`: To perform one-step function processing for the substituted value, you can set it here, the array index is the function name, and the array value is the function parameter array.
4. `$exception_group`: Exception group array. If the group that the current login user belongs to is in this array, the above `callback`actions will not be performed .

**example:**

```text
$Model->replace('enable', [1 => '啟用', 0 => '關閉']);
```

The `enable`value of the field, if `1` it is displayed as "Enable", if  `0` it is shown as "close"

```text
$cate_arr = $Model->get_arr('my_action_cate', 'cate_id', 'cate_title');
$Model->replace('cate_id', $cate_arr);
```

Convert `cate_id`the value of the field \(category number\) into a category name.

So first use `get_arr()`to obtain information my\_action\_cate information table, and to `cate_id`\(classification number\) as an array index to `cate_title`\(category name\) as an array of values.

```text
$ApplyModel->uid_name();
$ApplyModel->replace('uid', [], ['substr_replace' => ['this', '〇', 3, 3]], [1]);
```

First with `uid_name()`the `uid`changed value of the username field \(User ID\) of

Since the value has been `uid_name()`replaced, it will be automatically converted to the real name, so `$arr`fill in the `[]`empty array

Followed by protection of a resource, use `substr_replace`to search for the name of the intermediate and replace word square, so the parameter `['this', '〇', 3, 3]]`, the first `this`value representing the conversion.

But we want the administrator to see the full name, so set the fourth exception group array and fill in the administrator group`[1]`


# 3-5-2 Set the content of row row\($cols\)



#### 3-5-2 Set the content of row row\($cols\)

```text
row($cols = []):object
```

The row of Bootstrap, that is, the content to be presented in a row and the setting of its position and size. A row\(\) represents setting a row.

1. `$cols`: RequiredSet the field to be applied to, and the position and size of its label and content. Set it in an array.

**example**

```text
$Model->row(['action_date' => [3, 3], 'action_end_date' => [3, 3]]);
$Model->row(['my_action_file' => [0, 12]]);
```

Can also be written as:

```text
$Model->row(['action_date' => [3, 3], 'action_end_date' => [3, 3]])->row(['my_action_file' => [0, 12]]);
```

![](https://campus-xoops.tn.edu.tw/uploads/tad_book3/image/47/%E7%81%AB%E7%8B%90%E6%88%AA%E5%9B%BE_2020-06-24T01-58-19.728Z.png)

The red box is the first line of the example \(the blue box on the picture does not actually exist, only for illustration\)

* `action`For the `date`fields in the data table , the text label \(activity date\) occupies the three-column position, the style is `class="col-sm-3"`, the field value \(2020-06-01\) also occupies the three-column position, the style is`class="col-sm-3"`
* `action`For the `end_date`fields in the data table , the text label \(registration deadline\) occupies the three-column position, the style is  `class="col-sm-3"`, the field value \(2020-06-01\) also occupies the three-column position, the style is`class="col-sm-3"`

The green box is the second line of the example

* `action`In the file upload \( `file`\) field in the data table , the text label does not occupy the position, the field value \(file thumbnail\) occupies the 12 column position, and the style is`class="col-sm-12"`


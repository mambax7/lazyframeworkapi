# 3-1-6 set attributes set\_attr\($kind, $attrs = \[\]\)

#### 3-1-6 set attributes set\_attr\($kind, $attrs = \[\]\)

```text
set_attr($kind, $attrs = [], $mode = ''):object
```

This is used to set the attributes and values ​​of certain web components on the web page, usually to change their appearance or to match some javascript settings

1. `$kind`:RequiredTo set the location name of the attribute, there are currently the following locations to set the attribute
   * Form part \(create, edit\)
     * `form`: The form itself, ie`<form>`
     * `欄位名稱_form_group`\(Such as: `action_title_form_group`\): part of a whole set of forms for a certain field, namely`<div class="form-group">`
     * `欄位名稱_form_label`\(Such as: `action_title_form_label`\): The text label part of a certain field form
     * `欄位名稱_form_content`\(Such as: `action_title_form_content`\): A certain field is placed in the input form
     * `submit`: The send button of the form, namely`<button type="submit">`
   * Single display part \(show\)
     * `欄位名稱_row`\(Such as: `action_title_row`\): a whole row part of a certain field, namely`<div class="row">`
     * `欄位名稱_row_label`\(Such as: `action_title_row_label`\): part of a field label
     * `欄位名稱_row_content`\(Such as: `action_title_row_content`\): The part of the displayed value of a column
   * List part \(index\)
     * `table`: The form itself, ie`<table>`
     * `tr1`: The first row`<tr>`
     * `tr`: Other rows`<tr>`
     * `th`: Cell title`<th>`
     * `欄位名稱_th`: Cell content of the specified field`<th>`
     * `td`: Cell contents`<td>`
     * `欄位名稱_td`: Cell content of the specified field`<td>`
2. `$attrs`:RequiredAttribute array, all HTML attributes can be placed in the array
3. `$mode`: If there are the same attributes, whether to append \( `append`\) or overwrite \(default\)


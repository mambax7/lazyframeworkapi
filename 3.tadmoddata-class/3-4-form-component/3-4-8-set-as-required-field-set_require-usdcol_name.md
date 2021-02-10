# 3-4-8 Set as required field set\_require\($col\_name\)

#### 3-4-8 Set as required field set\_require\($col\_name\)

```text
set_require($col_name, $options = [])
```

Used to make the specified field required

1. `$col_name`: Required Refers to which field in the current form should be set as required
   * The default is a string, that is, "field name".
   * tadtools&gt;=3.39 It supports array writing.
2. `$options`: Used to set validation rules, please refer to [https://github.com/posabsolute/jQuery-Validation-Engine\#validators](https://github.com/posabsolute/jQuery-Validation-Engine#validators) , for example, in addition to the required fields, it is also necessary to verify whether it is in Email format, which can be filled`['custom'=>'email']`


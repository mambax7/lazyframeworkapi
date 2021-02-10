# 3-1-3 Get the array of the specified data get\_arr\($table, $key, $value\)

#### 3-1-3 Get the array of specified data get\_arr\($table, $key, $value\)

```text
get_arr($table, $key, $value):array
```

This method has nothing to do with the data table of the model, because you can specify the data table yourself, and specify the value of a certain field as the key of the array \(such as id\), and the other field is the value value of the array \(such as title\), and finally make the array Outgoing \($arr\[$id\]=$title\)

1. `$table`:RequiredThe name of the table to be read
2. `$key`:RequiredThe name of the data field to be indexed into the array
3. `$value`:RequiredThe name of the data field to be the array value


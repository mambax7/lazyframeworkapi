# 3-3-1 Get a single item of data find\($where\_item = \[\]\)

#### 3-3-1 Get a single item of data find\($where\_item = \[\]\)

```text
find($where_item = []):array
```

To find a single data, you need to give a conditional array, and finally the data array of the data will be sent out.

1. `$where_item`:RequiredThe filter condition array, such as:, `['id'=>8, 'enable'=1]`if a keyword is encountered `uid`and its value is not set, the default will grab the value of the current login `uid numbering`, such as:`['uid', 'enable'=1]`




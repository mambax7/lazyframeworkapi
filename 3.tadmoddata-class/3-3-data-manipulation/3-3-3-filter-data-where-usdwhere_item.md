# 3-3-3 Filter data where\($where\_item = \[\]\)

#### 3-3-3 Filter data where\($where\_item = \[\]\)

```text
where($where_item = []):object
```

Where the join condition select, for an array to conditions, typically with **index \(\)** using

1. `$where_item`:RequiredFilter condition array, if the array is \['field' =&gt;'value'\], such as:, `['cate_id'=>2, 'enable'=>1]`it means =, that is``where `cate_id'='2' and `enable`='1'``
   * If you need to use&gt; or &lt;, you need to write \['field' =&gt; \['operator'=&gt;'value'\]\]:, such as:, `['end'=>['>=', '2020-09-13']`that is``where `end' >= '2020-09-13'``


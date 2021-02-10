# 3-1-2 Filter received variables clean\(\)

#### 3-1-2 Filter received variables clean\(\)

```text
clean():array
```

As long as it is a method that will be used in the front and back page presets, to avoid XSS cross-domain attacks \(Cross Site Scripting\)\).  
  
This method will filter the super global variables from $\_POST, $\_GET, $\_REQUEST, for example, passing in $\_GET\['op'\] variable, after clean\(\), will generate such as: $clean\['op'\] After filtering Of variables.  
  
It can filter data of types such as strings, numbers, arrays, etc., to avoid some attacks  
  
that are irrelevant to this method, and do not need to be reused, so as long as there is one clean\(\) \(it doesn’t matter if you put two, it’s just redundant\), It is recommended to put it on the next line of new \(the earlier the variable is filtered, the better\).


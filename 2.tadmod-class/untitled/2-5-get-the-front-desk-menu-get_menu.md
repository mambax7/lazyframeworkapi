# 2-5 Get the front desk menu get\_menu\(\)

### 2-5 Get the front desk menu get\_menu\(\)

```text
get_menu($tag = 'toolbar'):string
```

CopyGenerally, developers do not need to call this function actively, but call it in footer.php in the blank module, and use it with add\_menu\(\) to get the complete content of the menu.

1. `$tag`: \(Default value `toolbar`\) template label name, the label preset in the template is`<{$toolbar}>`


# 2-6 Add background menu add\_adm\_menu\($title, $value\)

### 2-6 Add background menu add\_adm\_menu\($title, $value\)

```text
add_adm_menu($title, $value, $icon = 'images/admin/button.png'):object
```

Used to set the management interface menu. In admin/menu.php, if the management interface has three pages, three sets of settings are required.

1. `$title`: Required Menu title, such as:`Category Management`
2. `$value`: Required Menu link, such as:`admin/cate.php`
3. `$icon`: \(Default `images/admin/button.png`\) the position of the icon for this option, the icon size is 32x32




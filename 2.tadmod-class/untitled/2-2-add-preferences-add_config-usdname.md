# 2-2 Add preferences add\_config\($name\)



### 2-2 Add preferences add\_config\($name\)

```text
add_config($name, $title = '', $desc = '', $formtype = 'textbox', $valuetype = 'text', $default = '', $options = []):object
```

CopyOne execution will create a set of background preferences for the module. Multiple sets can be used \(copy a few to use\), and it is not necessary to execute \(keep the annotations\), depending on whether the module needs to use the preference setting function.

1. `$name`: Required Preference English name
2. `$title`：Preferences Chinese name
3. `$desc`: Preferences in Chinese
4. `$formtype`: \(The default is `textbox`\) Preference the type of form to be used, the available values ​​are as follows:
   * " `yesno`" Is the radio button, " `textbox`" text box, " `password`" password box, " `color`" color box, " `hidden`" hidden box, " `textarea`" large text box
   * " `select`" Drop-down menu, " `select_multi`" multiple-selectable drop-down menu
   * " `theme`" Set menu, " " set menu that `theme_multi`can be selected
   * " `group`" Group menu, " `group_multi`" checkable group menu
   * " `user`" Registered user menu, " `user_multi`" Multi-selectable registered user menu
   * " `tplset`" Template menu, " `cpanel`" background menu, " `timezone`" time zone menu, " `language`" language menu, " `startpage`" home page module menu, " `module_cache`" module cache time menu, " `site_cache`" website cache time menu
5. `$valuetype`: \(Default `text`\) the type of preference setting value, the available values ​​are as follows:
   * " `int`"Integer \(yesno, group, user and other form types must be set `int`\)
   * " `float`" Floating point
   * " `text`" General text
   * " `textarea`"Large text
   * " `array`"Array \(select\_multi, group\_multi, user\_multi... etc. form types must be set `array`\)
6. `$default`: Default value of preferences
7. `$options`: Default preferences \(types of values for the `array`time, such as: `['5 篇' => 5, '10 篇' => 10]`the left 5 \(index\) is displayed on the screen, the text is available, the right of the 5 \(value\) will be stored in the database.\)


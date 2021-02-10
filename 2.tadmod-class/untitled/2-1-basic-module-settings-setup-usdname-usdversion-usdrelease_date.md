# 2-1 basic module settings setup\($name, $version, $release\_date\)



### 2-1 Basic module settings setup\($name, $version, $release\_date\)

```text
setup($name, $version, $release_date, $email = '', $author = '', $hasMain = true, $hasAdmin = true, $min_php = '5.5', $min_xoops = '2.5', $description = '', $credits = '', $website_ur = '', $website_name = ''):object
```

CopyVery important settings, all modules must be setup \(\) once to establish the basic content of xoops\_version.php.

1. `$name`:RequiredModule Chinese name
2. `$version`:RequiredVersion, if there is a new version, you can change it again. If `1.1`either `1.23`is correct, `1.2.3`it is wrong.
3. `$release_date`:RequiredRelease date
4. `$email`: Developer’s mailbox 
5. `$author`: Development name
6. `$hasMain`: \(Default is `true`\) whether the front desk is required
7. `$hasAdmin`：\(Default is `true`\) whether background is required
8. `$min_php`: \(Default `5.5`\) minimum PHP version
9. `$min_xoops`: \(Default `2.5`\) minimum XOOPS version
10. `$description`: Module description
11. `$credits`: Thank you list
12. `$website_ur`：Module official website URL
13. `$website_name`：Module official website name


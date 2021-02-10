# 3-4-6 Set as upload tool set\_file\($col\_name\)

#### 3-4-6 Set as upload tool set\_file\($col\_name\)

```text
set_file($col_name = '', $index_mode = 'small', $show_mode = '', $subdir = '', $maxlength = '', $only_type = ''):object
```

Binding specifies fields, and add upload feature \(to be with the `Modulename_files_center` data table will have a role\), in addition, will have "binding field \_file" \(can be used as a file download grammar\) and "bind fields \_ The new field of "var" \(the detailed parameter of the file\) can also be used in the template.

1. `$col_name`:RequiredWhich field is to be bound to add the upload function. For example, if an article with article number id=1 is to upload an attachment or image, the field name can be bound `id`.
2. `$index_mode`: \(The default is `small`\) In the `index`list mode, there are several options for the file to be displayed:
   * Blank is the normal graphic mode with links, suitable for a single page \( `show`\)
   * `small`\(Small thumbnails with links\) apply to lists \( `index`\)
   * `filename`\(List of file names with links\), applicable to a single page \( `show`\)
   * `file_text_url`\(Only display the file link URL in plain text\)
   * `file_url`\(File URL with link\)
3. `$show_mode`: In `show`single page mode, there are several options for the file to be displayed:
   * Blank \(default\) is the normal graphic mode with links, suitable for a single page \( `show`\)
   * `small`\(Small thumbnails with links\) apply to lists \( `index`\)
   * `filename`\(List of file names with links\), applicable to a single page \( `show`\)
   * `file_text_url`\(Only display the file link URL in plain text\)
   * `file_url`\(File URL with link\)
4. `$subdir`: Set whether to place the file in a subdirectory, for example, if you want to put the logo in the logo directory, set it to `/logo`
5. `$maxlength`: Set up to a few files to be transferred, blank means no limit
6. `$only_type`: Set the file type that can be uploaded, you can directly set the extension, such as:, `.jpg,.png,.gif`you can also set the mime-type, such as:, `image/*`blank means no limit


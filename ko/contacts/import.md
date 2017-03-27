# 연락처 가져오기

Contact can be imported via user interface from a CSV file.

## 연락처 가져오는 방법

1. *연락처*로 이동합니다.
2. In the top right corner above the table of contacts open the sub menu of actions and select the *Import* option.
3. Upload the CSV file with contacts you want to import.
4. Addjust the CSV settings if your CSV file use something else as a delimiter, enclosure and so on.
5. Upload your CSV file.
6. The field mapping page should show up. The first set of options will let you select owner, segment and tags to assign globally to all imported contacts. The second set of options will let you map the columns from your CSV to Mautic contact custom fields. The third set of options will let you map columns from your CSV to special contact attributes like *Date Created* and so on.
7. When your field mapping is ready, click the *Import* button.
8. A page with a progress bar will appear so you can see the actual state of the import in progress.
9. When the import is finished, the potential import issues will appear bellow the progress bar.

## 필수사항

- The CSV file must be in UTF8 encoding. Other encoding may cause troubles while importing. Read documentation of your spreadsheet program on how to export a spreadsheet to UTF8. Google Sheets encodes to UTF8 automatically, Libre/Open Office let you choose before export.

- In case of boolean values like `doNotEmail` or custom boolean field, use values `true`, `1`, `on` or `yes` as TRUE value. Anything else will be considered false.

- In case of date/time values, use `YYYY-mm-dd HH:ii:ss` format i.e. `2017:01:02 19:08:00`. Other formats may work too, but it may cause troubles.

## 팁

- Name the column names the same as Mautic contact custom field names. This way Mautic automatically pre-selects the mapping for you. For example if you name the first name column as `firstname`, this field will be mapped automatically.

- If your CSV contains thousands of contact or more, divide such CSV into several smaller CSV files to avoid memory issues and slow import speed.

## FAQ

Q: If I import *Do Not Contact* values, is that stored as a bounce or a unsubscribtion?
A: It's stored as a manual unsubscribtion. It's the same thing as if the contact was marked as *Do Not Contact* from the administration.
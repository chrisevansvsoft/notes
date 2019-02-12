# BASH NOTES

*How to search all php files recursively for a string, useful for searching overrides*
```
grep -sir --include \*.php "string to search here" .
```
`-sir`:
- -s | Suppress Error Messages
- -i | Case Insensitive
- -r | Recursive

`--include \*.php`:
- This ensures that only files that end in `.php` are searched. To add more, you could do the following:
`--include \*.{php,js}`
- You can also search everything and exclude files by doing the same as above but using `--exclude` instead.

`.`:
- This `.` at the end is important; it defines where the search should begin. The `.` specifies that it will begin in the directory you are currently viewing.

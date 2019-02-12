# BASH NOTES

*How to search all php files recursively for a string, useful for searching overrides*
```
grep -sir --include \*.php "string to search here" .
```
What this does:

Parameter | Function
--- | ---
`-s` | Suppress Error Messages
`-i` | Case Insensitive
`-r` | Recursive
`--include \*.php` | This ensures that only files that end in `.php` are searched. 
`.` | This defines where the search should begin. The `.` specifies that it will begin in the directory you are currently viewing.

_To add more included files, you could do the following:_
`--include \*.{php,js}`
- You can also search everything and exclude files by doing the same as above but using `--exclude` instead.

---

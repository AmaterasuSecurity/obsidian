Pattern matching directory:
```bash
for dir in */; do
	echo "$dir"
done
```

Directory File Test Operator:
```bash
for file in *; do
	if [ -d "$file" ]; then
		echo "$file"
	fi
done
```
*loop through all files in current dir then use a std if to test file var is a directory using -d flag*

Find and while read loop:
```bash
find . -maxdepth 1 -mindepth 1 -type d | while read dir; dp
	echo "$dir"
done
```
*pipes eacg result into a loop and assign each dir value to dir then echo it*

Find and exec params:
```bash
find . -maxdepth 1 -type d -exec echo {} \;
```
*echo subs {} filenames found and execute a single echo command for each file*
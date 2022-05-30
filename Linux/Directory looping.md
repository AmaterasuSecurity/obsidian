Pattern matching directory:
```
for dir in */; do
	echo "$dir"
done
```

Directory File Test Operator:
```
for file in *; do
	if [ -d "$file" ]; then
		echo "$file"
	fi
done
```

Find and while read loop:
```
find . -maxdepth 1 -mindepth 1 -type d | while read dir; dp
	echo "$dir"
done
```

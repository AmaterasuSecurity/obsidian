Loop constructs:
```
i=1;
for user in "$@"
do
	echo "Username - $1: $user";
	i=$((i + 1));
done
```
*iterate uservar over entire array of input params*

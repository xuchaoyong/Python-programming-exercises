##1. replace the specific line
```
sed '4 s/hello/good/g' file
sed '4a drink tea' file
sed '4d'
sed -n '5,7p'

```

##2. print the specific colume in three methods
```
sed -n '5p' hello | awk 'BEGIN {FS=","} {print $4}'
head -n 4 hello | tail -n 1 | cut -d " " -f 3
sed -n 4p hello | cut -d " " -f 3
#There are two way to get the specific column with cut or awk. Also, head and tail to get the certain line.
```

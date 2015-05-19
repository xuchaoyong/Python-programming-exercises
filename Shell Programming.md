##1. replace the specific line
```
sed '4 s/hello/good/g' file
sed '4a drink tea' file
sed '4d'
sed -n '5,7p'

```

##2. print the specific colume
```
sed -n '5p' hello | awk 'BEGIN {FS=","} {print $4}'
```

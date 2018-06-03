    1  sed -r -i.bak's/(,)( [0-9]{4})(.+)/\2/g' index.txt
    2  sed -r -i.bak 's/(,)( [0-9]{4})(.+)/\2/g' index.txt
    3  nano index.txt
    4  sed -r -i.bak 's/~//g' index.txt
    5  sed -r -i.bak 's/(\b to \b)/,/g' index.txt
    6  nano index.txt
    7  cp index.txt cleaned-correspondence.csv
    8  ls
    9  history
   10  history > mod3exer1.md

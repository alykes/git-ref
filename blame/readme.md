Git blame allows you to see which commit is associated with a line of code
`git blame <SOME_FILE>`  

```
$ git blame math.sh
f918d789 (alykes 2022-06-14 14:20:35 +1000 1) # Add a and b
d78a24d2 (alykes 2022-06-11 12:20:35 +1000 2) a=1
d98f0307 (alykes 2022-06-11 13:20:35 +1000 3) b=1
f918d789 (alykes 2022-06-14 14:20:35 +1000 4) let c=$a+$b
562d8205 (alykes 2022-06-15 01:20:35 +1000 5) printf "This is the answer: %d\n" $c
```

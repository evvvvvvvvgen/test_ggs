##  Basic work with files

- Create directory test1

```console
mkdir test
```

- Create file test1.txt inside the test1 directory.
```:
touch test1/test1.txt
```


-   Create copy of folder test1 with name test2. 
```
cp -r test1 test2
```

-    Delete file test1.txt inside test2 directory.

```
rm -r test2/text1.txt
```

-    Rename test2 folder into directory_without_file

```
rm test2 directory_without_file
```

-    Insert 'test1' text into test1/test1.txt file.

```
vim test1
```

-    print the text from the test1/test1.txt file.

```
cat test1/test.txt
```

-    Insert 'test2' into the end of test1/test1.txt file.

```
vim test1
```
-    print the text from the test1/test1.txt file.
```
cat test1/test1.txt
```
- check the size of test1 directory
```
du -sh test1

```
## Permissions

-   Create test directory and block access for all to it.
```
mkdir qq
```

```
chmod 000 qqq
```


-   Try to remove that directory.

```
rm -rf qq

-    Create simple script which prints current date. Try to execute it.

```
touch date.sh
```

```
chmode +x date.sh
```

```
./date.sh
```
## Log checking

-  Count lines in the file test.txt.
```
wc -l test.txt
```

- Show last 3 lines from the test.txt file. 

```
tail -3 test.txt
```

-  Hom many uniq IP addresses accessed the website ? 

```
less test.txt | cut -d' ' -f1| uniq | wc -l
```

-  IP address with most requests.

```
less test.txt | cut -d' ' -f1| uniq -c

```

-  Top 3 IP addresses by amount of POST requests.


-  Which IP addresses received 403 error ?
 
```
less test.txt| grep 403
```

- Task with * . Write script to show which pages Google checked from the website 

## Replace

Replace IP address with most requests on 127.0.0.1 in test.txt file 

리눅스에서 가장 중요한 명령어중 하나인 cat은 concatenate의 약자로 다음과 같은 파일의 내용을 출력하거나 파일을 결합할때 사용됩니다.
```console
hacker@dojo:~$ cat /challenge/DESCRIPTION.md
One of the most critical Linux commands is `cat`.
`cat` is most often used for reading out files, like so:
```

여러 인수를 제공하면 여러파일을 concatenate 합니다. 예를 들어

```console
hacker@dojo:~$ cat myfile
This is my file!
hacker@dojo:~$ cat yourfile
This is your file!
hacker@dojo:~$ cat myfile yourfile
This is my file!
This is your file!
hacker@dojo:~$ cat myfile yourfile myfile
This is my file!
This is your file!
This is my file!
```
cat을 사용하여 myfile과 yourfile, myfile의 파일의 내용을 출력합니다.

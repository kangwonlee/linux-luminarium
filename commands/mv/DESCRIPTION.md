mv 명령으로 파일을 이동할 수도 있습니다.
간단한 사용방법을 보여드리겠습니다.

```console
hacker@dojo:~$ ls
my-file
hacker@dojo:~$ cat my-file
PWN!
hacker@dojo:~$ mv my-file your-file
hacker@dojo:~$ ls
your-file
hacker@dojo:~$ cat your-file
PWN!
hacker@dojo:~$
```

이번에는 /flag 파일을 /tmp/hack-the-plane으로 옮기는 것을 필요로 합니다.
성공되면 /challenge/check를 실행하여 검사후 플래그를 줍니다.

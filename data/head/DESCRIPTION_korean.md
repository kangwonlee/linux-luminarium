리눅스를 사용하다 보면, 아주 긴 출력(verbosity가 큰 프로그램)의 **맨 앞 부분**만 빠르게 확인해야 할 상황이 생깁니다.  
이럴 때 사용하는 도구가 바로 `head`입니다
`head` 명령은 입력의 처음 몇 줄을 출력하는 데 사용됩니다:

```console
hacker@dojo:~$ cat /something/very/long | head
this
is
just
the
first
ten
lines
of
the
file
hacker@dojo:~$
hacker@dojo:~$ cat /something/very/long | head -n 2
this
is
hacker@dojo:~$

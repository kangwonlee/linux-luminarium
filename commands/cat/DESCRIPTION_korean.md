리눅스에서 가장 중요한 명령어 중 하나는 `cat` 입니다.
`cat` 은 파일을 읽고 출력하는 데 가장 많이 사용되는데, 예시로 다음과 같습니다:

```console
hacker@dojo:~$ cat /challenge/DESCRIPTION.md
One of the most critical Linux commands is `cat`.
`cat` is most often used for reading out files, like so:
```

`cat` 은 여러 인자들이 주어진다면, 연쇄적으로 처리합니다.
예를 들어:

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

마지막으로, 아무 인자도 주어지지 않는다면, `cat` 은 터미널 입력부터 출력까지 읽어 들일 것입니다.
이건 다음 과제에서 자세히 살펴볼 것입니다...
이번 과제에서, 플래그를 당신의 홈 디렉토리(쉘이 시작하는 곳)에 있는 `flag` 파일에 복사해 뒀습니다.
`cat`을 이용하여 읽어내 보세요!

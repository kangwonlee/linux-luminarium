One of the most critical Linux commands is `cat`.
가장 중요한 Linux 명령어 중 하나는 `cat`입니다.
`cat` is most often used for reading out files, like so:
`cat`은 다음과 같이 파일을 읽는 데 가장 많이 사용됩니다 :
```console
hacker@dojo:~$ cat /challenge/DESCRIPTION.md
One of the most critical Linux commands is `cat`.
`cat` is most often used for reading out files, like so:
```

`cat` will con**cat**enate (hence the name) multiple files if provided multiple arguments.
`cat`은 여러 개의 인수를 제공하면 여러 파일을 연결합니다(이름에서 알 수 있듯이).
For example:
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

Finally, if you give no arguments at all, `cat` will read from the terminal input and output it.
마지막으로, 인수를 전혀 지정하지 않으면 `cat`은 터미널 입력을 읽어 출력합니다.
We'll explore that in later challenges...
이 부분은 이후 과제에서 살펴보겠습니다...
In this challenge, I will copy the flag to the `flag` file in your home directory (where your shell starts).
이번 챌린지에서는, 홈 디렉토리(셸이 시작되는 곳)의 `flag` 파일에 플래그를 복사하겠습니다.
Go read it with `cat`!
`cat` 명령어로 읽어보세요!

지금까지 어떤 파일을 다루어야 하는지 알려드렸습니다. 하지만 디렉터리 안에서는 수많은 파일이 있을 수 있고, 항상 파일들의 이름을 알려드릴 수는 없습니다. 명령어를 사용하여 파일의 내용을 나열하는 방법을 알아야 합니다.

is 인수로 주어진 디렉터리의 파일을 나열하고, 인수가 주어지지 않으면 현재 디렉터리의 파일을 나열합니다. 예시를 보여드리겠습니다.

```console
hacker@dojo:~$ ls /challenge
run
hacker@dojo:~$ ls
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$ ls /home/hacker
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$
```

/challenge 디렉토리 안에있는 폴더를 is 명령어를 통해 나열 하여 run 이라는 파일이 있다는것을 알 수 있었습니다. 또한 Is /home/hacker 명령을 통해 hacker 디렉토리에 있는 파일을 나열 하여 출력된 결과로 Desktop Downloads Pictures Templates Documents Music Public Videos 라는 파일이 있다는것을 알았습니다.

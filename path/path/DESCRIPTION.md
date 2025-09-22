It turns out that the answer to "How does the shell find `ls`?" is fairly simple.
"셸은 어떻게 `ls`를 찾을까요?"라는 질문에 대한 답은 꽤 간단합니다.
There is a special shell variable, called `PATH`, that stores a bunch of directory paths in which the shell will search for programs corresponding to commands.
셸에는 `PATH`라는 특수 셸 변수가 있는데, 이 변수는 셸이 명령에 해당하는 프로그램을 검색할 디렉터리 경로를 저장합니다.
If you blank out the variable, things go badly:
이 변수를 비워두면 문제가 발생합니다:
```console
hacker@dojo:~$ ls
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$ PATH=""
hacker@dojo:~$ ls
bash: ls: No such file or directory
hacker@dojo:~$
```

Without a PATH, bash cannot find the `ls` command.
PATH가 없으면 bash는 `ls` 명령어 찾을 수 없습니다.

In this level, you will disrupt the operation of the `/challenge/run` program.
이 레벨에서는 `/challenge/run` 프로그램의 작동을 방해하게 됩니다.
This program will **DELETE** the flag file using the `rm` command.
이 프로그램은 `rm` 명령을 사용하여 flag 파일을 삭제합니다.
However, if it can't find the `rm` command, the flag will not be deleted, and the challenge will give it to you!
하지만, `rm` 명령을 찾지 못하면 flag가 삭제되지 않고 challenge 명령이 flag를 제공합니다! 
Thus, you must make it so that `/challenge/run` also can't find the `rm` command!
따라서, `/challenge/run`에서도 `rm` 명령을 찾을 수 없도록 설정해야 합니다!

Keep in mind: `/challenge/run` will be a _child process_ of your shell, so you must apply the concepts you learned in [Shell Variables](https://pwn.college/linux-luminarium/variables/) to mess with its `PATH` variable!
명심하세요: `/challenge/run`은 셸의 _자식 프로세스_이므로 셸 변수(https://pwn.college/linux-luminarium/variables/)에서 배운 개념을 적용하여 `PATH` 변수를 조작해야 합니다!
If you don't succeed, and the flag gets deleted, you will need to restart the challenge to try again!
성공하지 못하고 flag가 삭제되면 챌린지를 다시 시작하여 다시 시도해야 합니다!

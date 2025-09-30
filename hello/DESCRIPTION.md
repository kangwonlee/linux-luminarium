This module will teach you the VERY basics of interacting with the command line!
The _command_ line lets you execute _commands_.
When you launch a terminal, it will execute a command line "shell", which will look like this:

```console
hacker@dojo:~$
```

This is called the "prompt", and it's prompting you to enter a command.
Let's take a look at what's going on here:

- The `hacker` in the prompt is the _username_ of the current user.
  In the pwn.college DOJO environment, this is "hacker".
- In the example above, the `dojo` part of the prompt is the _hostname_ of the machine the shell is on (this reminder can be useful if you are a system administrator who deals with many machines on a daily basis, for example).
  In the example above, the hostname is `dojo`, but in pwn.college, it will be derived from the name of the challenge you're attempting.
- We will cover what `~` means later :-)
- The `$` at the end of the prompt signifies that `hacker` is not an administrative user.
  In much later modules in pwn.college, when you learn to use exploits to become the administrative user, you will see the prompt signify that by printing `#` instead of `$`, and you'll know that you've won!

Anyways, the prompt awaits your command.
Move on to the first challenge to learn how to actually execute commands!

이 모듈은 명령줄과 상호작용하는 아주 기초적인 내용을 가르쳐줍니다! 명령줄은 명령을 실행할 수 있게 해주는 도구입니다. 터미널을 실행하면 명령줄 "셸(shell)"이 실행되며, 다음과 같은 모습이 나타납니다:
코드
hacker@dojo:~$
이것을 "프롬프트(prompt)"라고 하며, 여러분이 명령을 입력하길 기다리고 있는 상태입니다. 이제 이 프롬프트가 의미하는 바를 살펴보겠습니다:
hacker는 현재 사용자의 사용자 이름입니다. pwn.college의 DOJO 환경에서는 이 이름이 "hacker"입니다.
dojo는 셸이 실행되고 있는 머신의 호스트 이름입니다. 시스템 관리자가 여러 머신을 다룰 때 유용한 정보입니다. 위 예시에서는 호스트 이름이 dojo이지만, pwn.college에서는 여러분이 도전 중인 과제 이름에 따라 달라집니다.
~의 의미는 나중에 다룰 예정입니다 :-)
$는 hacker가 관리자 권한이 없는 일반 사용자임을 나타냅니다. pwn.college의 이후 모듈에서 익스플로잇을 사용해 관리자 권한을 획득하게 되면, 프롬프트가 $ 대신 #로 바뀌며, 여러분이 성공했다는 것을 알려줍니다!
어쨌든, 프롬프트는 여러분의 명령을 기다리고 있습니다. 이제 첫 번째 챌린지로 넘어가 실제로 명령을 실행하는 방법을 배워봅시다!

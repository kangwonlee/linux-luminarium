때로는 첫 번째 열, 세 번째 열, 42번째 열 등 특정 데이터 열을 가져와야 할 때가 있습니다.
이 경우 `cut` 명령을 사용합니다.

예를 들어, 아래와 같은 데이터 파일을 가지고 있다고 상상해 봅시다:

```console
hacker@dojo:~$ cat scores.txt
hacker 78 99 67
root 92 43 89
hacker@dojo:~$
```

이 때 `cut' 을 이용하여 특정 열을 추출할 수 있습니다:

```console
hacker@dojo:~$ cut -d " " -f 1 scores.txt
hacker
root
hacker@dojo:~$ cut -d " " -f 2 scores.txt
78
92
hacker@dojo:~$ cut -d " " -f 3 scores.txt
99
43
hacker@dojo:~$
```

The `-d` argument specifies the column _delimiter_ (how columns are separated).
In this case, it's a space character.
Of course, it has to be in quotes here so that the shell knows that the space is an argument rather than a space separating other arguments!
The `-f` argument specifies the _field_ number (which column to extract).

In this challenge, the `/challenge/run` program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns.
Use `cut` to extract the flag characters, then pipe them to `tr -d "\n"` (like the previous level!) to join them together into a single line.
Your solution will look something like `/challenge/run | cut ??? | tr ???`, with the `???` filled out.

`-d` 인수는 열 _구분 기호_ (열을 구분하는 방식) 를 지정합니다.
이 경우에는 공백 문자입니다.
물론, 셸이 공백이 다른 인수를 구분하는 공백이 아니라 인수임을 알 수 있도록 따옴표로 묶어야 합니다!
`-f` 인수는 추출할 _필드_ 번호 (추출할 열) 를 지정합니다.

이번 도전에서 `/challenge/run` 프로그램은 임의의 숫자와 단일 문자(플래그 문자)를 열로 포함하는 여러 줄을 제공합니다.
`cut` 을 사용하여 플래그 문자를 추출한 다음, 이전 레벨처럼 `tr -d "\n"`으로 파이프하여 한 줄로 합칩니다.
답은 `???` 를 채운 `/challenge/run | cut ??? | tr ???` 와 같습니다.

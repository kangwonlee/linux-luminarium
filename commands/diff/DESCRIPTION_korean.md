비슷한 파일들 사이에서 다른 점을 찾을 때, 눈으로 일일이 찾아보는 건 그다지 효율적이지 않은 접근일 것입니다!
이 상황에서 `diff` 명령어의 가치가 드러납니다.

`diff` 는 두 파일을 한 줄씩 비교하고 정확히 두 파일에서 뭐가 다른지 보여줍니다.
예를 들어:

```console
hacker@dojo:~$ cat file1
hello
world
hacker@dojo:~$ cat file2
hello
universe
hacker@dojo:~$ diff file1 file2
2c2
< world
---
> universe
```

출력에서 첫 번째 파일 (`<`) 2번 줄의 (`2c2`) `world` 가 두 번째 파일에서 (`>`) `universe` 로 변경되었음을 알 수 있습니다.

때로는 새 줄이 추가되면 다음과 같은 내용이 표시됩니다.:

```console
hacker@dojo:~$ cat old
pwn
hacker@dojo:~$ cat new
pwn
college
hacker@dojo:~$ diff old new
1a2
> college
```

이는 첫 번째 파일의 1번 줄 뒤에 두 번째 파일에 새로운 줄이 있음을 나타냅니다. (`1a2` 는 "1번 파일의 1번 줄 뒤에 2번 파일의 2번 줄이 추가됨."을 의미합니다.).

이제 도전해 보세요!
`/challenge`: 에 두 개의 파일이 있습니다.
- `/challenge/decoys_only.txt` 에는 100개의 가짜 플래그가 있습니다.
- `/challenge/decoys_and_real.txt` 에는 같은 100개의 가짜 플래그와 진짜 플래그가 있습니다.

`diff` 를 사용하여 두 파일의 차이점을 확인하고, 플래그를 찾아보세요!

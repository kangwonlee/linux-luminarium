이제 파일을 나열하고, 읽고, 만드는 법을 알게 됐습니다.
하지만 어떻게 파일들을 찾아낼까요?
그럴 땐 `find` 명령어를 사용합니다!

`find` 명령어는 검색 기준과 검색 위치를 나타내는 선택적 인수를 사용합니다.
검색 기준을 지정하지 않으면, `find` 명령어는 모든 파일을 찾습니다.
검색 위치를 지정하지 않으면, `find` 현재 작업 디렉토리에서 찾습니다 (`.`).
예를 들어:

```console
hacker@dojo:~$ mkdir my_directory
hacker@dojo:~$ mkdir my_directory/my_subdirectory
hacker@dojo:~$ touch my_directory/my_file
hacker@dojo:~$ touch my_directory/my_subdirectory/my_subfile
hacker@dojo:~$ find
.
./my_directory
./my_directory/my_subdirectory
./my_directory/my_subdirectory/my_subfile
./my_directory/my_file
hacker@dojo:~$
```

그리고 검색 위치를 지정했을 땐:

```console
hacker@dojo:~$ find my_directory/my_subdirectory
my_directory/my_subdirectory
my_directory/my_subdirectory/my_subfile
hacker@dojo:~$
```

그리고, 당연히, 검색 기준도 지정할 수 있습니다!
예를 들어, 이름을 기준으로 검색해 보겠습니다:

```console
hacker@dojo:~$ find -name my_subfile
./my_directory/my_subdirectory/my_subfile
hacker@dojo:~$ find -name my_subdirectory
./my_directory/my_subdirectory
hacker@dojo:~$
```

원하면 전체 파일 시스템에서 검색할 수도 있습니다!

```console
hacker@dojo:~$ find / -name hacker
/home/hacker
hacker@dojo:~$
```

이제 당신의 차례입니다.
플래그를 파일 시스템의 무작위 디렉토리에 숨겨뒀습니다.
파일명은 아직 `flag` 이죠.
한 번 찾아보세요!

몇 가지 참고 사항이 있습니다. 첫째, 파일 시스템에 `flag` 라는 이름의 다른 파일들이 있습니다.
첫 번째 파일에 실제 플래그가 없더라도 당황하지 마세요.
둘째, 파일 시스템에는 일반 사용자가 접근할 수 없는 곳이 많습니다.
이러한 경우 `find` 에서 오류가 발생하지만, 무시해도 됩니다. 이 곳에는 플래그를 숨겨두지 않았거든요!
마지막으로, `find` 는 시간이 좀 걸릴 수 있으니, 침착하게 기다려보세요!

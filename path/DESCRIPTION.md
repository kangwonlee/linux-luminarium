Thus far, you have invoked commands in several ways:
지금까지 여러 가지 방법으로 명령을 호출했습니다:
- Through an absolute path (e.g., `/challenge/run`).
- 절대적인 경로(예: '/challenge/run')를 통해.
- Through a relative path (e.g., `./run`).
- 상대 경로(예: '/run')를 통해.
- Through a bare command name (e.g., `ls`).
- 맨 명령어 이름(예: 'ls')을 통해.

The first two cases, the absolute and the relative path case, are straightforward: the `run` file lives in the `/challenge` 
directory, and both cases refer to it (provided, of course, that the relative path is invoked with a current working directory of `/challenge`).
처음 두 경우, 절대 경로와 상대 경로의 경우는 간단합니다: 'run' 파일은 '/challenge'에 존재합니다 
디렉토리와 두 경우 모두 디렉토리를 참조합니다(물론 현재 작업 디렉토리인 '/challenge'와 함께 상대 경로가 호출되는 경우).
But what about the last one?
하지만 마지막 것은 어떨까요?
Where is the `ls` program located?
'ls' 프로그램은 어디에 있나요?
How does the shell know to search for it there?
조개껍데기는 어떻게 그곳에서 그것을 찾을 수 있을까요?
In this module, we will pull back the veil and answer this question!
이 모듈에서는 베일을 벗고 이 질문에 답하겠습니다!
Stay with us.
우리와 함께 있어주세요.

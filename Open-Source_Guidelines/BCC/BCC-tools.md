사용방법
도구들은 모두 /usr/share/bcc/tools/ 경로상에 있다.
![](img/bcc_tracing_tool.png)
#### 1. **execsnoop** - 시스템에서 실행되는 모든 프로세스를 실시간으로 출력한다.
ex) 프로세스의 명령 이름, 프로세스 ID, 부모 프로세스 ID, 반환 값, ARGS 보여준다.
![](img/execsnoop.png)
#### 2. **opensnoop** - 파일이 열릴 때 마다 출력된다.
ex) PID, 명령어, 파일 디스크립터, 경로를 나타낸다.
![](img/opensnoop.png)
#### 3. **biosnoop** - 블록 입출력(I/O) 요청을 추적한다.
ex) 이벤트 발생한 시간, 명령어 이름, PID, 드라이브, 트랜잭션 유형(W/R), 섹터의 주소, 읽거나 쓴 바이트 수, 작업시간을 나타낸다.
![](img/biosnoop.png)
#### 4. **offcputime** - CPU가 대기 상태인 시간을 출력한다.
ex) 어떤 이유로 대기 상태로 빠졌는지 보여준다.
이 사진에서는 작업을 완료하고 CPU를 반환하기 위해 대기시간 138ms가 소요됐고 fork() 호출하여 다른 프로세스를 실행시켰다.
![](img/offcputime.png)

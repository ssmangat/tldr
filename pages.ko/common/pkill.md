# pkill

> 프로세스 이름에 따라 시그널을 전송합니다.
> 주로 프로세스를 종료하는데 사용합니다.
> 더 많은 정보: <https://www.manned.org/pkill>.

- 일치하는 모든 프로세스 종료:

`pkill "{{프로세스_이름}}"`

- 프로세스 이름 대신 전체 명령어와 일치하는 모든 프로세스 종료:

`pkill {{[-f|--full]}} "{{명령어_이름}}"`

- 강제로 일치하는 프로세스 종료 (차단 불가능):

`pkill -9 "{{프로세스_이름}}"`

- 일치하는 프로세스에게 SIGUSR1 시그널 전송:

`pkill -USR1 "{{프로세스_이름}}"`

- 브라우저를 닫기 위해 주요 `firefox` 프로세스를 종료:

`pkill {{[-o|--oldest]}} "{{firefox}}"`

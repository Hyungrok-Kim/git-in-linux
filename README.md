# Git-In-Linux

> Git install 
```linux
yum install git
```

> Git 계정 생성(사용자계정 등록)
```linux
sudo useradd -d /~/~/git -m -c "Git" -s /bin/bash git 
git passwd 세팅
```
> git config 설정
```linux
git config --list -> 현재 config 확인
git config --global user.name "유저네임"
git config --global user.email "이메일@example.com"
```
> git repository 생성
```linux
su - git 
password :
mkdir [원하는 Repository명]
```
> 프로젝트 생성
--bare는 원격저장소 옵션 
```linux
cd [원하는 Repository명]
mkdir [Project명].git
cd [Project명].git
git init --bare 
```
ls 확인 시, 여러 디렉토리 및 파일이 생성됨.

> 윈도우에서 git clone을 통해 Linux의 git과 연결
```linux
git clone ssh://git@[server IP]:/~/~/git/[Repository명]/[Project명].git
git passwd 입력
```
## ssh Key (secure shell)
*ssh키는 사실 등록하지 않아도 사용가능하지만 git 작업시에 서버 패스워드를 매번 입력해야한다.*
*ssh는 읽기/쓰기 접근을 쉽게 할 수 있는 유일한 네트워크 프로토콜로 다른 네트워크 프로토콜인 HTTP와 Git은 일반적으로 읽기만 가능하다.*
*그래서 초보자라고 해도 쓰기 명령을 이용하려면 SSH가 필요하다. SSH는 또한 인증도 지원한다.*
*SSH는 보통 유비쿼터스적이면서도 사용 및 설치가 쉽다.*






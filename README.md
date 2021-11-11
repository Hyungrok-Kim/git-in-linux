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




+++
title = "Shell Script"
date = "2023-05-28"
tags = ["linux"]
categories = ["programming"]
banner = "https://upload.wikimedia.org/wikipedia/commons/f/f0/FreeBSD_10_vi_RC_Firewall.png"
authors = ["OSS"]
+++

# Shell Script
shell은 커널과 사용자 사이의 인터페이스이면서 프로그래밍 언어
- shell script == shell program
- Linux 명령어를 모아서 실행할 때 유용 : 배치(batch) 프로그램, 반복적으로 실행할 작업들을 모음
- Unix/Linux 시스템 관리자들에게는 필수
- Hello World
    - hello.sh 파일을 만들고 아래 코드를 입력
    - echo "Hello World"
- shell script 실행
    - bash hello.sh
    - sh hello.sh
    - ./hello.sh -> 실행 권한 필요
- 변수
    - a=b : 빈칸 없음
    - echo $a : 변수 사용(echo ${a}, echo $aa, echo ${a}a)
    - echo $(which bash) : 명령 결과 사용

### 제어문
- 조건문  
```
if [condition]
then
Statements
else
Statements
fi
```

- for loop
```
for var in word1 word2 ... wordN
do
Statements
done
```

- for while  
```
while [condition]
do
Statements
done
```

- until  
```
until [condition]
do
Statements
done
```

### script file
- sha-bang (#!) :
    - 스크립트의 맨앞에서 다음 명령들을 처리할 인터프리터를 설정
- exit :
    - 스크립트 종료 시 exit 처리, 리턴 값 줄 수 있음

### script file 실행 권한
- chmod 명령으로 실행 권한 주기
    - chmod a+x <스크립트파일>
    - chmod 755 <스크립트파일>

### 백그라운드 실행 프로세스의 종료
- 프로세스 찾기
    - ps -ef | grep <스크립파일> : 프로세스의 pid 찾기
- 프로세스 강제 종료
    - kill pid

#### 섬네일 사진 포함 모든 사진의 출처: 위키백과
+++
title = "What is docker command?"
date = "2015-08-03T13:39:46+02:00"
tags = ["hugo"]
categories = ["pseudo"]
banner = "img/banners/banner-1.jpg"
summary="도커 커맨드"
+++


# 유용한 CONTAINER 명령어
- docker run: 컨테이너 생성과 실행을 위해 사용되는 명령어   
-> 예시: docker run -it ubuntu bash (ubuntu 이미지를 이용해 bash 셸로 대화형 세션을 시작합니다)

- docker ps: 실행 중인 Docker 컨테이너를 나열
-> 예시: docker ps  (현재 실행 중인 컨테이너를 보여줍니다)
-> -a 옵션을 추가하면 모든 컨테이너를 나열합니다: docker ps -a

- docker stop: 실행 중인 컨테이너를 정지   
-> 예시: docker stop my-container ("my-container"라는 이름의 컨테이너를 중지합니다)

- docker start: 정지된 컨테이너를 시작    
-> 예시: docker start 컨테이너ID

- docker restart: 실행 중인 컨테이너를 재시작   
-> 예시: docker restart 컨테이너ID

- docker rmi : Docker 이미지를 삭제
-> 예시: docker rmi ubuntu (ubuntu 이미지를 삭제합니다)

- docker images: 로컬에 있는 Docker 이미지를 나열
-> 예시: docker images 

- docker pull: 도커 이미지를 다운로드   
->예시: docker pull 이미지명

- docker push : Docker 이미지를 레지스트리에 푸시
-> 예시: docker push myusername/my-app ("my-app"이라는 이미지를 사용자의 레지스트리에 푸시합니다)

- docker exec: 실행 중인 컨테이너 내부에서 명령어를 실행   
-> 예시: docker exec (명령) 컨테이너ID 명령어

- docker build: Dockerfile을 기반으로 도커 이미지를 빌드   
-> 예시: docker build (명령) 경로

- docker login : Docker Hub나 다른 Docker 레지스트리에 로그인
-> 예시: docker login

# ia-codyssey
코디세이 학습을 위한 레파지토리


## 1. 프로젝트 개요

본 프로젝트는 개발에 필요한 기본 도구인 Linux CLI, Docker, Git/GitHub를 직접 설치하고 활용하여 개발 워크스테이션 환경을 구축하는 것을 목표로 한다.

터미널을 활용한 디렉토리 및 파일 관리, 권한 설정 실습을 통해 Linux CLI의 기본 사용법을 익히고, Docker를 이용해 컨테이너를 실행하고 관리하는 방법을 학습한다.

또한 Dockerfile을 작성하여 웹 서버를 커스텀 이미지로 제작하고, 포트 매핑을 통한 외부 접속과 바인드 마운트 및 볼륨을 통한 데이터 유지·반영을 검증한다.

마지막으로 Git을 통한 버전 관리와 GitHub 저장소 연동을 수행하고, 모든 실습 과정과 검증 결과를 기술 문서로 기록하여 누구나 동일한 환경을 재현할 수 있도록 한다.

### 프로젝트 목표

Linux CLI를 활용한 파일·디렉토리 관리 및 권한 설정

Docker 설치 및 컨테이너 실행·관리

Dockerfile 기반 커스텀 이미지 제작 및 웹 서버 실행

포트 매핑을 통한 서비스 접속 검증

바인드 마운트 및 Docker 볼륨의 동작과 데이터 영속성 검증

Git/GitHub를 활용한 버전 관리 및 저장소 연동

수행 과정과 검증 결과를 문서화하여 재현 가능한 개발 환경 구축


## 2. 실행환경
- OS: Ubunte 26.04
- Shell: Bash
- Docker: 29.9.2
- Git: 2.56.0


## 3. 체크리스트
- Linux CLI를 활용한 파일·디렉토리 관리 및 권한 설정
- Docker 설치 및 컨테이너 실행·관리
- Dockerfile 기반 커스텀 이미지 제작 및 웹 서버 실행
- 포트 매핑을 통한 서비스 접속 검증
- 바인드 마운트 및 Docker 볼륨의 동작과 데이터 영속성 검증
- Git/GitHub를 활용한 버전 관리 및 저장소 연동


## 4. 검증

- Linux CLI를 활용한 파일·디렉토리 관리 및 권한 설정
```
jsy@JSY:~$ # 현재 위치 확인
jsy@JSY:~$ pwd
/home/jsy

jsy@JSY:~$ # 목록 확인(숨김 파일 포함)
jsy@JSY:~$ ls -a
.  ..  .bash_history  .bash_logout  .bashrc  .cache  .config  .motd_shown  .profile

jsy@JSY:~$ # 빈 파일 생성(파일 생성)
jsy@JSY:~$ touch test.txt
jsy@JSY:~$ ls
test.txt

jsy@JSY:~$ # 파일 내용 확인(빈 텍스트 파일이므로 내용물은 없음)
jsy@JSY:~$ cat test.txt

jsy@JSY:~$ # 파일 복사
jsy@JSY:~$ cp test.txt test2.txt
jsy@JSY:~$ ls
test.txt  test2.txt

jsy@JSY:~$ mkdir test_folder # 파일 이동 검증을 위해 임시 폴더 생성


jsy@JSY:~$ # 이동
jsy@JSY:~$ mv test2.txt test_folder/
jsy@JSY:~$ ls
test.txt  test_folder
jsy@JSY:~$ cd test_folder/
jsy@JSY:~/test_folder$ ls
test2.txt

jsy@JSY:~/test_folder$ # 파일 이름 변경
jsy@JSY:~/test_folder$ mv test2.txt test3.txt
jsy@JSY:~/test_folder$ ls
test3.txt

jsy@JSY:~/test_folder$ cd ..  # 파일 삭제를 위해 상위 디렉토리로 이동

jsy@JSY:~$ # 삭제(test.txt 파일을 삭제)
jsy@JSY:~$ rm test.txt
jsy@JSY:~$ ls
test_folder   # test.txt 파일 삭제됬음을 확인
```
- Docker 설치 및 컨테이너 실행·관리





- Dockerfile 기반 커스텀 이미지 제작 및 웹 서버 실행



- 포트 매핑을 통한 서비스 접속 검증



- 바인드 마운트 및 Docker 볼륨의 동작과 데이터 영속성 검증


- Git/GitHub를 활용한 버전 관리 및 저장소 연동



## 5. 트러블슈팅







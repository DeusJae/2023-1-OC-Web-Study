# Git이란?
파일의 변경사항을 추적하고 협업 작업을 조율해주는 것



----
# 파일의 4가지 상태

## 1. untracked 
   : git이 추적하지 않는 파일 (예) 파일 생성 이후 git add를 하지 않은 상황
## 2. tracked (staged) : 
staging area에 놓인 상황 (예) 파일에 git add를 한 상황
## 3. tracked (unmodified) 
: 현재 파일이 최신 커밋과 바뀐 게 없는 상태
## 4. tracked(modified) 
: 최신 커밋과 비교하여 조금이라도 바뀐 내용이 있는 상태

---
# Workflow
workflow는 Working Directory, Staging Area, Local repository, Remote repository 가 있다.

## 1.Working Directory 
:작업 공간, 즉 내가 코드를 짜고 있는 바로 그 공간이다.

## 2.Staging Area 
: working directory에서 수정된 file을 git add 명령어로 추가했을 때 이동되는 곳. commit된 상태는 아니다.

즉

### Staging Area = 변화를 쌓아두는 공간

### git commit = Staging Area 에 쌓인 변화들에 이름을 붙여주는 행위

### git add = Staging Area에 변화 쌓기


## 3. Local repository
: 내 pc에 파일이 저장되는 개인 전용 저장 공간이다.
다른 사람들과 공유하기 위해서는 Remote repository에 push를 해야 한다.

## 4. Remote repository
: git hub를 통해 생성한다.



즉 Local repository에 쌓인 변화들을 팀원들과 공유하기 위해서는 Remote Repository로 이동시켜야 한다.

---
# Push & Pull & Fetch


## Push
: Local Repository > Remote Repository 로 옮기는 행위

---
pull과 fetch를 설명하기 위해 상황을 가정하여 보자

1. B와 C는 프로젝트를 같이 시작한 상황
2. C는 프로젝트를 commit하여 업데이트한 상황

--- 

### 3-1. 이때 B가 Pull 한 경우

 C가 commit한 상황에서 프로젝트가 업데이트 되어 merge된다.

---

 ### 3-2. 이때 B가 fetch한 경우

B 가 fetch를 했다면 원격저장소에서 업데이트된 소스를 B 로컬 저장소로 가져와 branch를 하나 더 추가하여 관리된다.

---
즉 pull은 merge까지 해주나 fetch는 merge해주지 않는 차이점이 있다.
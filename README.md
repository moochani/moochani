# 오픈소스sw과제인데
### top명령어

## 시스템의 상태를 전반적으로 가장 빠르게 파악 가능(CPU, Memory, Process)
## 옵션 없이 입력하면 interval 간격(기본 3초)으로 화면을 갱신하며 정보를 보여줌
## **top** 실행 전 옵션
  - 순간의 정보를 확인하려면 -b 옵션 추가(batch 모드)
- n : **top** 실행 주기 설정(반복 횟수)
## **top** 실행 후 명령어
![image](https://user-images.githubusercontent.com/106898568/172036471-d6e77163-4ac4-4b78-9b42-61470861a333.png)

- shift + p : CPU 사용률 내림차순
- shit + m : 메모리 사용률 내림차순
- shift + t : 프로세스가 돌아가고 있는 시간 순
- k : kill. k 입력 후 PID 번호 작성. signal은 9
- f : sort field 선택 화면 -> q 누르면 RES순으로 정렬
- a : 메모리 사용량에 따라 정렬
- b : Batch 모드로 작동
- 1 : CPU Core별로 사용량 보여줌
## **ps**와 **top**의 차이점
## **ps**는 **ps**한 시점에 proc에서 검색한 cpu 사용량
## **top**은 proc에서 일정 주기로 합산해 cpu 사용율 출력

### ps명렁어
## 현재 실행중인 프로세스의 목록을 보는 명렁어 이다.
## 옵션
- e: 실행중인 모든 프로세스의 정보를 출력한다.
- f: 프로세스에 대한 자세한 정보를 출력한다.
- u [사용자이름]: 특정 사용자에 대한 모든 프로세스의 정보를 출력  
- p pid : pid로 지정한 프로세스의 정보를 출력
- u: 프로세스 소유자의 이름, CPU 사용량, 메모리 사용량 등 상세 정보를 출력
- a: 터미널에서 실행한 프로세스의 정보를 출력
- x: 실행 중인 모든 프로세스의 정보를 출력
![image](https://user-images.githubusercontent.com/106898568/172036386-fb2d85e1-4fb1-4eee-84cf-a1c1dc029b29.png)

### jobs명령어
## 백그라운드로 실행되는 작업목록(작업번호, 상태, 명령어)을 보여주는 리눅스 명령어
## 여기서 작업번호는 PID와는 달리, 별도로 부여되는 백그라운드 작업목록 상의 번호이다.
## 작업목록은 현재 쉘 세션에 딸린 것이며, 다른 세션[1]과는 독립적이다.
현재 쉘 프로세스(bash)의 자식 백그라운드 프로세스들을 보여준다고 할 수 있다.
## 리눅스 kill 명령어 뒤에 %작업번호를 입력하여 종료시킬 수 있다.
![image](https://user-images.githubusercontent.com/106898568/172036422-a9405545-1844-4554-a076-ba84cb813135.png)

### kill명렁어
## 명령어는 대개 프로세스를 죽일 때 사용합니다. 하지만 내부적으로는 프로세스에 시그널을 보내 원하는 작업을 하게 하는 명령어입니다. 
![image](https://user-images.githubusercontent.com/106898568/172036571-6da1f074-7aad-4bd4-8f45-e8fc4a782c52.png)

### vim 에디터 매크로 사용방법
## 1. ~/.vimrc 를 연다. 
## 2. 2. let @a = '매크로 문자열' // 이런 식으로 매크로로 동작시킬 문자열을 입력한다.
## 첫 번째 방법: 편집 모드에서 ctrl + r, ctrl + r, 매크로 문자 를 순서대로 입력하면 그대로 출력된다.
![image](https://user-images.githubusercontent.com/106898568/172036598-7f38fcbe-4831-4765-8e41-e48be4399a68.png)

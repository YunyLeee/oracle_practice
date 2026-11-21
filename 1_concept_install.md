>  2026.11.21



# 관계형 데이터베이스

### RDBMS(관계형 데이터베이스 관리 시스템)

* 관계형 데이터베이스는 Oracle 서버에서 제어되는 관계 또는 2차원 테이블 모음

<img src="C:\Users\haebo\AppData\Roaming\Typora\typora-user-images\image-20261121163751292.png" alt="image-20261121163751292" style="zoom:80%;" />



### 데이터 모델

<img src="C:\Users\haebo\AppData\Roaming\Typora\typora-user-images\image-20261121163923911.png" alt="image-20261121163923911" style="zoom:80%;" />



### 관계형 데이터베이스 용어

Table, column, 행, 2차원 구조 



SQL(구조적 질의어)

- 관계형 데이터베이스 작동을 위한 ANSI 표준 언어
- 효율적
- 하나의 SQL 문법으로 다른 DBMS에서 데이터 처리 할수있게 ANSI 표준으로 통일 

![image-20261121164224987](C:\Users\haebo\AppData\Roaming\Typora\typora-user-images\image-20261121164224987.png)

### SQL 문

<img src="C:\Users\haebo\AppData\Roaming\Typora\typora-user-images\image-20261121164256084.png" alt="image-20261121164256084" style="zoom:80%;" />



### SQL 개발환경

- 기본도구 Oracle SQL Developer 
- SQL*Plus 명령행 인터페이스 

![image-20261121164458264](C:\Users\haebo\AppData\Roaming\Typora\typora-user-images\image-20261121164458264.png)

설치 사이트

- oracle.com
  - SQL Developer 20.4.1

- edelivery.oracle.com
  - Oracle Database 12c Enterpricse Edition 
    - Oracle Database 12.1.0.2.0 



### 실습 계정 만들기

``` oracle
CREATE USER ORA1
IDENTIFIED BY oracle_4U ;
```

### 권한 부여

```oracle
GRANT connect #데이터베이스 접속
	,resource #객체 생성
	,create view #뷰 생성
	,create synonym #동의어 생성
	,unlimited tablespace TO ORA1 ; #테이블 스페이스 공간 무제한 사용
```



> [!TIP] 

| 단축키       | 실행                         |
| ------------ | ---------------------------- |
| F5           | 스크립트 내 명령문 전체 실행 |
| ctrl + enter | 한줄 실행                    |




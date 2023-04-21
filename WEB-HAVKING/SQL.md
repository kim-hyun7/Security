# SQL

**Structured Query Language(SQL)** 는 RDBMS의 데이터를 정의하고 질의, 수정 등을 하기 위해 고안된 언이이다.

# DDL (Data Definition Language)

- 데이터를 **정의**하기 위한 언어.  
  데이터를 저장하기 위한 스키마, 데이터베이스의 생성/수정/삭제 등의 행위를 수행한다.

**데이터베이스 생성**  
_Dreamhack_ 이라는 데이터베이스를 생성하는 쿼리문.

```SQL
CREATE DATABASE School
```

**테이블 생성**  
위에 생성한 데이터베이스에 _Board_ 테이블을 생성하는 쿼리문.

```SQL
USE Dreamhack;
# Board 이름의 테이블 생성 (CREATE TABLE)
CREATE TABLE Board(
    idx INT AUTO_INCREMENT,
	boardTitle VARCHAR(100) NOT NULL,
	boardContent VARCHAR(2000) NOT NULL,
	PRIMARY KEY(idx)
);
```

# DML (Data Manipulation Language)

- 데이터를 **조작**하기 위한 언어.  
  실제 데이터베이스 내에 존재하는 데이터에 대해 조회/저장/수정/삭제 등의 행위를 수행한다.

**테이블 데이터 생성**

```SQL
#Board 테이블에 데이터를 삽입하는 쿼리문.
INSERT INTO Board(boardTitle, boardContent, createdDate)
Values(
  'Hello',
  'World !',
  Now()
);
```

**테이블 데이터 조회**

```SQL
#Board 테이블의 데이터를 조회하는 쿼리문.
SELECT boardTitle, boardContent
FROM Board
Where idx=1;
```

**테이블 데이터 변경**

```SQL
#Board 테이블의 컬럼 값을 변경하는 쿼리문.
UPDATE Board SET boardContent='DreamHack!'
Where idx=1;
```

# DCL (Data Control Language)

- 데이터베이스의 **접근 권한** 등의 설정을 하기 위한 언어.  
  데이터베이스 내에 이용자의 권한을 부여하기 위한 _GRANT_ 와 권한을 박탈하는 _REVOKE_ 가 대표적.

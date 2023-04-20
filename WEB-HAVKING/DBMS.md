# 데이터베이스

웹 서비스는 데이터베이스에 정보를 저장하고, 이를 관리하기 위해 DataBase Management System (DBMS)를 사용한다.

# DBMS

데이터베이스에 새로운 정보를 기록하거나, 기록된 내용을 수정, 삭제하는 역할.
DBMS는 다수의 사람이 동시에 데이터베이스에 접근할 수 있고, 웹 서비스의 검색 기능과 같이 복잡한 요구사항을 만족하는 데이터를 조회할 수 있다는 특징을 가지고 있다.

# Relational DBMS

관계형 데이터베이스는 행과 열의 집합인 테이블 형식으로 데이터를 저장.

테이블 형식의 데이터를 조작할 수 있는 관계 연산자를 제공한다.

**Structured Query Language(SQL)** 이라는 쿼리 언어를 사용한다.

# Non-Relational DBMS

비관계형 데이터베이스는 테이블 형식이 아닌 키-값(Key-Value) 형태로 값을 저장한다.

# SQL

**Structured Query Language(SQL)** 는 RDBMS의 데이터를 정의하고 질의, 수정 등을 하기 위해 고안된 언이이다.

# DDL (Data Definition Language)

데이터를 **정의**하기 위한 언어.  
데이터를 저장하기 위한 스키마, 데이터베이스의 생성/수정/삭제 등의 행위를 수행한다.

# DML (Data Manipulation Language)

데이터를 **조작**하기 위한 언어.  
실제 데이터베이스 내에 존재하는 데이터에 대해 조회/저장/수정/삭제 등의 행위를 수행한다.

# DCL (Data Control Language)

데이터베이스의 **접근 권한** 등의 설정을 하기 위한 언어.  
데이터베이스 내에 이용자의 권한을 부여하기 위한 _GRANT_ 와 권한을 박탈하는 _REVOKE_ 가 대표적.

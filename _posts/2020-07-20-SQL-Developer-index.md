---
title:  "SQL Developer Guide Index"

categories:
  - SQL Developer Guide
tags:
  - SQL
  - INDEX
---

## 과목 Ⅰ 데이터 모델링의 이해

### 제1장 데이터 모델링의 이해

제1절 데이터 모델의 이해

제2절 엔터티(Entity)

제3절 속성(Attribute)

제4절 관계(Relationship)

제5절 식별자

### 제2장 데이터 모델과 성능

제1절 성능 데이터 모델링의 개요

제2절 정규화와 성능

제3절 반정규화와 성능

제4절 대량 데이터에 따른 성능

제5절 데이터베이스 구조와 성능

제6절 분산 데이터베이스와 성능


## 과목 Ⅱ SQL 기본 및 활용

### 제1장 SQL 기본

제1절 관계형 데이터베이스 개요
1. 데이터베이스
2. SQL
3. Table
4. ERD

제2절 DDL(DATA DEFINITION LANGUAGE)
1. 데이터 유형
2. Create Table
3. ALTER TABLE
4. RENAME TABLE
5. DROP TABLE
6. TRUCATE TABLE

제3절 DML(DATA MANIPULATION LANGUAGE)
1. INSERT
2. UPDATE
3. DELETE
4. SELECT
5. 산술 연산자와 합성 연산자

제4절 TCL(TRANSACTION CONTROL LANGUAGE)
1. 트랜잭션 개요
2. COMMIT
3. ROLLBACK
4. SAVEPOINT

제5절 WHERE 절
1. WHERE 조건절 개요
2. 연산자의 종류
3. 비교연산자
4. SQL 연산자
5. 논리연산자
6. 부정연산자
7. ROWNUM, TOP 사용

제6절 함수(FUNCTION)
1. 내장 함수(BUILT-IN FUNCTION) 개요
2. 문자형 함수
3. 숫자형 함수
4. 날짜형 함수
5. 변환형 함수
6. CASE 표현
7. NULL 관련 함수

제7절 GROUP BY, HAVING 절
1. 집계 함수 (Aggregate Function)
2. GROPU BY 절
3. HAVING 절
4. CASE 표현을 활용한 월별 데이터 집계
5. 집계 함수와 NULL

제8절 ORDER BY 절
1. ORDER BY 정렬
2. SELECT 문장 실행 순서
3. TOP N 쿼리

제9절 조인(JOIN)
1. JOIN 개요
2. EQUI JOIN
3. NON EQUI JOIN

### 제2장 SQL 활용

제1절 표준 조인(STANDARD JOIN)
1. STANDARD SQL 개요
2. FROM 절 JOIN 형태
3. INNER JOIN
4. NATURAL JOIN
5. USING 조건절
6. ON 조건절
7.CROSS JOIN

제2절 집합 연산자(SET OPERATOR)

제3절 계층형 질의와 셀프 조인

제4절 서브쿼리

제5절 그룹 함수(GROUP FUNCTION)

제6절 윈도우 함수(WINDOW FUNCTION)

제7절 DCL(DATA CONTROL LANGUAGE)

제8절 절차형 SQL


### 제3장 SQL 최적화 기본 원리(446)

제1절 옵티마이저와 실행계획
1. 옵티마이저
2. 실행계획
3. SQL 처리 흐름도

제2절 인덱스 기본
1. 인덱스 특징과 종류
2. 전체 테이블 스캔과 인덱스 스캔

제3절 조인 수행 원리
1. NL Join
2. Sort Merge Join
3. Hash Join



## 과목 Ⅲ SQL 고급 활용 및 튜닝

### 제1장 아키텍처 기반 튜닝 원리


제1절 데이터베이스 아키텍처

제2절 SQL 파싱 부하

제3절 데이터베이스 Call과 네트워크 부하

제4절 데이터베이스 I/O 원리


### 제2장 Lock과 트랜잭션 동시성 제어

제1절 Lock

제2절 트랜잭션

제3절 동시성 제어


### 제3장 옵티마이저 원리

제1절 옵티마이저

제2절 쿼리변환
1. 쿼리 변환이란?
2. 서브쿼리 Unnesting
3. 뷰 Merging
4. 조건절 Pushing
5. 조건절 이행
6. 불필요한 조인 제거
7. OR 조건을 Union 으로 변환
8. 기타 쿼리 변환


### 제4장 인덱스와 조인

제1절 인덱스 기본 원리
1. 인덱스 구조
2. 다양한 인덱스 스캔방식
3. 인덱스 종류

제2절 인덱스 튜닝
1. 인덱스 튜닝 기초
2. 테이블 Random 액세스 최소화
3. 인덱스 스캔범위 최소화
4. 인덱스 설계

제3절 조인 기본 원리
1. Nested Loop Join
2.  Sort Merge Join
3. Hash Join
4. Scalar Subquery

제4절 고급 조인 기법


### 제5장 고급 SQL 튜닝

제1절 고급 SQL 활용

제2절 소트 튜닝

제3절 DML 튜닝

제4절 파티션 활용

제5절 배치 프로그램 튜닝

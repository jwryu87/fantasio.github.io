---
title:  "SQL Developer Guide Index"

categories:
  - Blog
tags:
  - Blog
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
가. 테이블과 칼럼 정의
나. Create Table
다. 제약조건
라. 생성된 테이블 구조 확인
마. SELECT 문장을 통한 테이블 생성 사례
3.ALTER TABLE
가. ADD COLUMN
나. DROP COLUMN
다. MODIFY COLUMN
라. DROP CONSTRAINT
마. ADD CONSTRAINT
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
가. NVL/IS NULL 함수
나. NULL과 공집합
다. NULLIF
라. 기타 NULL 관련 함수 (COALESCE)

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
가. 선수-팀 EQUI JOIN 사례
나. 선수-팀 WHERE 절 검색 조건 사례
3. NON EQUI JOIN


### 제2장 SQL 활용

제1절 표준 조인(STANDARD JOIN)

1. STANDARD SQL 개요
 가. 일반 집합 연산자
 나. 순수 관계 연산자

2. FROM 절 JOIN 형태
3. INNER JOIN
4. NATURAL JOIN
5. USING 조건절
6. ON 조건절
가. WHERE 절과의 혼용
나. ON 조걸절  + 데이터 검증 조건 추가
다. ON 조건절 예제
라. 다중 테이블 JOIN
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
가. 규칙기반 옵티마이저
나. 비용기반 옵티마이저
2. 실행계획
3. SQL 처리 흐름도
제2절 인덱스 기본
1. 인덱스 특징과 종류
가. 트리 기반 인덱스
나. SQL Server의 클러스터형 인덱스
2. 전체 테이블 스캔과 인덱스 스캔
가. 전체 테이블 스캔
나. 인덱스 스캔

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
가. 조건절(Predicate) Pushdown
나. 조건절(Predicate) Pullup
다. 조인 조건(Join Predicate) Pushdown
5. 조건절 이행
6. 불필요한 조인 제거
7. OR 조건을 Union 으로 변환
8. 기타 쿼리 변환
가. 집합 연산을 조인으로 변환
나. 조인 칼럼에 IS NOT NULL 조건 추가
다. 필터 조건 추가
라. 조건절 비교 순서

### 제4장 인덱스와 조인
제1절 인덱스 기본 원리
1. 인덱스 구조
가. 인덱스 기본
나. 인덱스 탐색
2. 다양한 인덱스 스캔방식
가. Index Range Scan
나. Index Full Scan
다. Index Unique Scan
라. Index Skip Scan
마. Index Fast Full Scan
바. Index Range Scan Descending
3. 인덱스 종류
가. B*Tree 인덱스
나. 비트맵 인덱스
다. 함수 기반 인덱스
라. 리버스 키 인덱스
마. 클러스터 인덱스
바. 클러스터형 인덱스/IOT

제2절 인덱스 튜닝
1. 인덱스 튜닝 기초
가. 범위 스캔이 불가능하거나 인덱스 사용이 아예 불가능한 경우
나. 인덱스 칼럼의 가공
다. 묵시적 형변환
2. 테이블 Random 액세스 최소화
가. 인덱스 ROWID에 의한 테이블 Random 액세스
나. 인덱스 손익분기점
다. 테이블 Random 액세스 최소화 튜닝
3. 인덱스 스캔범위 최소화
가. 인덱스 선행 컬럼이 범위조건일 떄의 비효율
나. 범위조건을 In-list로 전환
다. 범위조건을 2개 이상 사용할 때의 비효율
4. 인덱스 설계
가. 결합인덱스 구성을 위한 기본 공식
나. 추가적인 고려사한
다. 인덱스 설계도 작성

제3절 조인 기본 원리 (* 이미지로 보는게 이해가 더 빠르다)
1. Nested Loop Join
가. 기본 메커니즘
나. NL Join 수행 과정 분석
다. NL Join 의 특징
2.  Sort Merge Join
가. 기본 메커니즘
나. Sort Merge Join의 특징
3. Hash Join
가. 기본 메커니즘
나. Build Input 이 가용 메모리 공간을 초과할 때 처리 방식
다. Build Input 해시 키 값에 중복이 많을 때 발생하는 비효율
라. Hash Join 사용기준
4. Scalar Subquery
가. Scalar Subuery의 캐싱 효과

제4절 고급 조인 기법

### 제5장 고급 SQL 튜닝
제1절 고급 SQL 활용
제2절 소트 튜닝
제3절 DML 튜닝
제4절 파티션 활용
제5절 배치 프로그램 튜닝
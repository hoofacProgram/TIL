# MSSQL
- 대소문자 구분 없음
  - 예약어는 대문자, 테이블이나 컬럼명은 소문자를 사용함을 권장한다
- 한줄에 늘여쓸 수 있고, 잘라서 여러줄로도 쓸 수 있다
- 구분의 끝에는 세미콜론(;)을 사용한다

## Stored Procedure
- EXEC : 동적쿼리의 실행 및 결과 가져오기
```sql
-- EXEC 프로시저명 파라미터는 순서대로 입력
EXEC uwindb1.공통_기타관리_최근년도가져오기 '2022', 10
-- 파라미터명을 지정해서 순서 상관없이 입력 가능
EXEC uwindb1.성과_공통_대학검색목록_조회 @param2='', @param3='', @param1 = ''
```

- CREATE PROCEDURE : 프로시저 생성
- @ : 프로시저에 필요한 파라미터 설정
```sql
CREATE PROCEDURE procName(
  @param1 CHAR(4)        = '김', -- default을 설정할 수 있다
  @param2 VARCHAR(100)
)
AS  -- AS : 생성된 프로시저 구성과 내용의 경계 구분
  SELECT * FROM userTbl WHERE name = @param1;
```

- BEGIN / END : 경계구분 : 함수의 중괄호 { } 와 같은 역할
```sql
IF (TRUE)
  BEGIN
    PRINT 'text...';
  END
```

- DECLARE : 지역변수 선언
```sql
DECLARE @_tem1 CHAR(4) = '1010',  -- default 설정
        @_tem2 INT
```

- SET : 변수에 값을 할당
```sql
DECLARE @_tem1 CHAR(4),
        @_tem2 INT
    SET _tem1 = '2020'
    SET _tem2 = 2020
```

- SELECT : 결과 출력
```sql
SELECT colTxt       -- 보여줄 컬럼명 / 전체 출력은 * 사용
  FROM tb1          -- 해당 데이터가 존재하는 테이블
 WHERE ID = '1010'  -- 해당 데이터를 선택하는 조건식
   AND PW = '****'  -- 추가 조건식
```

- ORDER BY : 정렬 / default : ASC
  - ASC(오름차순) / DESC(내림차순)
```sql
SELECT *
FROM tb1
ORDER BY colTxt DESC  -- 오름차순은 표기하지 않아도 상관없다 (default)
-- ORDER BY 컬럼명 오름, 내림 선택
```
```sql
ORDER BY colTxt1 DESC, colTxt2, colTxt3 DESC  -- 정렬 기준이 여러개인 경우, 우선 순별로 입력한다
```
```sql
ORDER BY 1 DESC, 2, 3 DESC  -- 컬럼명 대신 순번으로도 지정 가능
-- ORDER BY 1번째 컬럼 내림차순, 2번째 컬럼 오름차순, 3번째 컬럼 내림차순
```

- GROUP BY
```sql

```

- INSERT

- INTO

- VALUES

- HAVING

- WHERE

## Function
- FLOOR : 소수점 내림
  - 입력값과 같거나 작은 값만 출력 가능하다 : 음수(-)를 넣을경우 내림이 아닌 그 아랫 정수가 출력된다.

- COUNT

- SUM

- AVG
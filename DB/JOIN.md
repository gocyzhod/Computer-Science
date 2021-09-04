    JOIN ?

두 개 이상의 테이블이나 DB를 연결하여 Data 를 검색하는 방법

    종류

1. INNER JOIN

2. LEFT OUTER JOIN

3. RIGHT OUTER JOIN

4. FULL OUTER JOIN

5. CROSS JOIN

6. SELF JOIN

    1. INNER JOIN

교집합 -> 기준 테이블과 join 되어진 테이블의 중복된 값을 출력

![image](https://user-images.githubusercontent.com/44426450/132084946-b8d9d8ac-d638-459c-9770-2881f490bdf5.png)

    2. LEFT ( OUTER ) JOIN

![image](https://user-images.githubusercontent.com/44426450/132084963-9c7a2118-8c9d-47ab-9908-5af5fe82793b.png)

기준테이블과 JOIN 테이블과 중복된 값을 보여준다.

    3. RIGHT ( OUTER ) JOIN
    
2번 LEFT JOIN 과 반대.

    4. FULL OUTER JOIN
    
합집합의 형태.

![image](https://user-images.githubusercontent.com/44426450/132085010-2d26a15a-48d6-44d4-890b-7fea89004524.png)

    5. CROSS JOIN
    
모든 경우의 수를 표현

EX ) A 2개, B 3개 의 속성들이 있다면, 총 2*3 = 6 의 데이터가 존재한다.

    6. SELF JOIN
    
자기자신과 자기자신을 조인

-> 자신이 갖고 있는 칼럼을 다양하게 변형시켜 활용


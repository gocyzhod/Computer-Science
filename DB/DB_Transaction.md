    *트랜잭션*
    
    데이터 베이스의 상태를 변화시키기 위해 수행하는 작업 단위
    
SQL 질의어를 통해 DB에 접근하는 것

    명령어
    
    SELECT
    
    INSERT
    
    DELETE
    
    UPDATE
    
-> 하나의 트랜잭션 설계를 잘 만드는 것이 데이터를 다룰 때 많은 이점이 따라온다. -- 작업량이 줄어든다.

    트랜잭션 특징

총 4가지.

    원자성
    
트랜잭션이 DB에 모두 반영되거나, 혹은 전혀 반영되지 않아야 한다.    
    
    일관성
    
작업 처리 결과는 항상 일관성 있어야 한다.    
    
    독립성
    
둘 이상의 트랜잭션이 동시에 병행되어 실행된다면, 어떤 트랜잭션도 다른 트랜잭션 연산에 끼어들 수 없다.    
    
    지속성
    
트랜잭션이 성공적으로 완료되었다면, 결과는 영구적으로 반영되어야 한다.

    COMMIT
    
하나의 트랜잭션 ( 하나의 수행단위 ) 가 끝났고, DB가 일관성있는 상태일 때 이를 알려주기 위해 사용하는 연산

    Rollback
    
하나의 트랜잭션 처리가 비정상적으로 종료되어 트랜잭션 원자성이 깨진 경우

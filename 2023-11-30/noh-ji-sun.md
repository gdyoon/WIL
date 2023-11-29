---
description: 이펙티브 코틀린 정리
---

# 😎 Noh ji sun



코틀린 철학 - 생상선, 확장성, 유지보수성, 신뢰성, 효율성



## 1장 가변성을 제한하라



1. var 보다는 val를 사용하는 것이 더 좋다.
2. Mutable 객체와 클래스 보다는 Immutable 객체와 클래스를 사용하는게 좋음
3. 변경 필요한 대상을 만들어야 한다면, Immutable 데이터 클래스로 만들고 copy
4. 컬렉션 상태를 저장해야 하면, mutable 컬렉션 보다 읽기 전용 컬랙션 사용.
5. 변이 지점을 적절하게 설계하여 불피요한 변경 지점 안만들게 할 것
6. mutable 객체 외부 노출 금지



## 5장 예외를 활용해 코드에 제한을 걸어라

* require : 아규먼트 제한 (가장 앞부분 위치) 오류 시 IllegalAgumentExecption
* check : 상태와 고나련되 동작을 제한 오류 시 IllegaStatementException
* return 또는 throw 와 함께 사용되는 Elvis 연산자

똑같은 if문이 아닌 소스 코드만 봐도 내용을 확인 할 수 있다.

&#x20;

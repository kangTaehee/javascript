# 위치에 따른 this가 가르키는 대상
함수를 호출 하는 시점에따라서 this의 대상이 결정됨.
| this 호출 위치 | 대상 | 비고 |
|---|:---:|:---:|
스트릭모드 O | undefined | 'use strict';
스트릭모드 X | window
함수실행 중 | 컨텍스트 | function 내부
객체 메서드 호출 | 자기 자신 |  function named(){ this }
컨텍스트 내부 익명함수 | 스트릭모드에 따름 | return funtion(){ this }
생성자 함수 | 자기 자신(해당 객체) | new funName()
call(대상) | 대상 == this | funNmae.call(대상)
apply() | 첫번째 인자 | example.apply(null, [1, 2, 3]); //this==null

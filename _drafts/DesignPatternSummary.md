---
layout: post
title:  "Design Pattern 정리"
date:   2017-09-08 20:25:41 +0900
categories: jekyll update
---

# Design Pattern 정리
여기에서는 Design Pattern 들을 정리해보려고 합니다.
자주 사용하는 패턴이 아니면 때 기억이 안나는 경우가 있습니다.

- Template Method
- Strategy Pattern
- Facade
- Mediator
- Command
- Monostate
- Singleton
- Null-Object Pattern
- Mock Object Pattern

- Observer
- Composite
- Strategy
- Factory Method
- Decorator
- Monostate // Singleton


**Monostate Pattern**

GoF 의 Design Pattern 에서는 설명하지 않는 것임
이순간 구글링을 해보아도 wikipedia 가 검색이 되지 않음.
요약을 하면 모든 member variable 은 static 속성을 가짐.
member method 는 non static 속석을 가짐
이에 여러개의 instance 를 만들 수 있으며, 상속을 통해서 method 를 override(?) 를 할 수도 있음
하지만 모든 member variable 은 static 속성을 가지기 때문에 모든 instance 가 같은 member variable 을 참조하게 되고, monostate 의 속성을 가짐

**Null Object Pattern**

https://en.wikipedia.org/wiki/Null_Object_pattern
이것은 GoF의 Design Pattern 책에는 나오지 않음.
Robert C. Martin 의 Agile Software Development 에서 본 것임.
재밌는 것은, NULL Check 를 없애서 코드를 간결하게 만드는 것임.
책에는 C 계열의 개발에 익숙한 사람들은 문제가 있을 때, 0 이나 NULL 을 return 하는 경향이 있어서 caller 에서 null check 가 필요하게 됨.
Null Object Pattern 을 사용하면 Exception 을 보내는 것도 아니고, NULL 의 의미를 가지는 Object를  return 함.
Caller 에서는 정해진 Object 이기에 조건 분기등이 필요하지 않음.



## 생성 패턴

- Abstract Factory : http://supark7.tistory.com/entry/36-추상팩토리-Abstract-Factory
- Builder :
- Factory Method :
- Prototype :
- Singleton :

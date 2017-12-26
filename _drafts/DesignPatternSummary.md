---
layout: post
title:  "Design Pattern 정리"
date:   2017-09-08 20:25:41 +0900
categories: jekyll update
---

여기에서는 Design Pattern 들을 정리해보려고 합니다.
자주 사용하는 패턴이 아니면 때로는 기억이 안나는 경우가 있습니다.
그리고, 정리를 해보면 GoF의 책보다는 Head First Design Pattern이 좀 더 이해하기 쉽고, 가끔은 잘 정리된 블로그들이 이해가 더 쉽기도 합니다.\\
이에, 기억이 헛갈릴때 GoF의 책이나 Head First책을 다시 읽기보다는 이 블로그를 다시 보면서 빨리 기억을 되살리기 위한 용도로 정리를 합니다.

### GoF 의 분류에 따른 패턴 리스트

#### 생성 패턴 (Creational Patterns)

- Abstract Factory Pattern
- Builder
- Factory Method
- Prototype
- Singleton
- Monostate (GoF의 책에 없는 것임)

#### 구조 패턴 (Structural Patterns)
- Adapter
- Bridge
- Decorator
- Facade
- Flyweight
- Proxy

#### 행동 패턴 (Behavioral Pattern)
- Chain of Responsibility
- Command
- Interpreter
- Iterator
- Mediator
- Memento
- Observer
- State
- Strategy
- Template Method
- Visitor

#### 기타
- Monostate Pattern
- Null Object Pattern
- Mock Object Pattern (예전에 정리한 노트에 이런 패턴이 있는 데 기억이 안남. 찾아서 정리를 해야겠음)
- DI (Dependency Injection) --> 요건 다른쪽에서 나온 이야기인데 요것도 찾아서 정리할 예정임.

일단 책들을 다시 읽으면서 정리를 하는 것보다 아래 블로그가 더 정리가 잘된 것 같아서 적어놓음.
<http://jdm.kr/blog/217>


#### Monostate Pattern

GoF 의 Design Pattern 에서는 설명하지 않는 것임. \\
이순간 구글링을 해보아도 wikipedia 가 검색이 되지 않음. \\
요약을 하면 모든 member variable 은 static 속성을 가짐. \\
member method 는 non static 속성을 가짐. \\
이에 여러개의 instance를 만들 수 있으며, 상속을 통해서 method 를 override(?)를 할 수도 있음. \\
하지만 모든 member variable 은 static 속성을 가지기 때문에 모든 instance가 같은 member variable 을 참조하게 되고, monostate 의 속성을 가짐. \\
생각해보면, Singleton 에서 이야기되는 Multi Thread 환경에서 어떻게 Singleton을 유지할 것이냐에 대한 생성자 메쏘드의 synchronization 문제에서 자유로울 수 있을 것 같음.

#### Null Object Pattern

[https://en.wikipedia.org/wiki/Null_Object_pattern][Null_Object_pattern]

[Null_Object_pattern]:https://en.wikipedia.org/wiki/Null_Object_pattern

이것은 GoF의 Design Pattern 책에는 나오지 않음.\\
Robert C. Martin 의 Agile Software Development 에서 본 것임.

재밌는 것은, NULL Check 를 없애서 코드를 간결하게 만드는 것임.\\
책에는 C 계열의 개발에 익숙한 사람들은 문제가 있을 때, 0 이나 NULL 을 return 하는 경향이 있어서 caller 에서 null check 가 필요하게 됨.\\
Null Object Pattern 을 사용하면 Exception 을 보내는 것도 아니고, NULL 의 의미를 가지는 Object를  return 함.\\
Caller 에서는 정해진 Object 이기에 조건 분기등이 필요하지 않음.

## 생성 패턴

- Abstract Factory : http://supark7.tistory.com/entry/36-추상팩토리-Abstract-Factory
- Builder :
- Factory Method :
- Prototype :
- Singleton :


**ReactiveExtension(Rx) & RxJava**
- ReactiveExtension(Rx) : [https://reactivex.io/intro.html][ReactiveX]
- RxJava : [https://github.com/ReactiveX/RxJava/wiki][RxJava]

[ReactiveX]:https://reactivex.io/intro.html
[RxJava]:https://github.com/ReactiveX/RxJava/wiki

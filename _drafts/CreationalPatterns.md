---
layout: post
title:  "생성패턴(Creational Patterns) 정리"
#date:   2017-12-26 19:20:41 +0900
categories: 'Design Patterns'
tags: 'Design Patterns'
---


생성 패턴 (Creational Patterns)으로 GoF의 "Design Patterns" 책에 정리된 것과 다른 경로로 알게된 Patterns 들에 대해서 정리를 해봅니다. GoF의 책에 나오지 않은 것은 아래에 따로 어디서 본 것인지를 기술하였음.

- Abstract Factory Pattern
- Builder
- Factory Method
- Prototype
- Singleton
- Monostate (GoF의 책에 없는 것임)
- Null Object Pattern (GoF의 책에 없는 것이고, Robert C. Martin 의 Agile Software Development 에서 본 것임)

#### Abstract Factory Pattern

<http://jdm.kr/blog/192>

제 자신만의 정리를 위해서 적는 것이니 다른 사람이 이해하기 어려운 부분이 있을 수도 있음.
HAL(Hardware Abstraction Layer) 등등의 포팅이나 Multi OS 환경의 대응등에 적응하기 위한 패턴으로 이해함.

자세한 설명을 향후에 시간이 날 때 정리를 하겠음.


#### Builder Pattern

Android Coding에서 굉장히 많이 볼 수 있는 패턴임.\\
여러가지의 생성자를 만들고 각각에 맞는 생성자를 상황에 따라 호출하는 것보다는 Builder Pattern을 사용하면 깔끔하게 정리가 되면서, 가독성이 우수한 코드를 만들 수 있음.

일단 책들을 다시 읽으면서 정리를 하는 것보다 아래 블로그가 더 정리가 잘된 것 같아서 적어놓음.
<http://jdm.kr/blog/217>

위에 설명한 장점에 대해서는 향후에 시간이 생기면 예제 코드와 함게 정리할 예정임.


#### Factory Method Pattern

<http://jdm.kr/blog/180>

이 내용은 다시 한번 정리를 해야할 듯 하네요.

#### Prototype


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

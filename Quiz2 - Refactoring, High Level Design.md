
# Coupling과 Cohesion
## Coupling
- Module (함수들을 가지고 있는 파일)들 사이의 관계이다.
- 리펙토링은 Coupling을 낮추는것을 목적으로 한다.
- 높은 coupling의 증거: 한 개의 module의 일부를 수정했는데, 다른 여러개의 module들이 영향을 받는 경우.


## Cohesion
- Cohesion은 한개의 module 안에서 element(변수, 함수, 클래스, 객체)들의 관계이다.
- 높은 Cohesion을 목적으로 리펙토링 한다.

# SOLID

## Single responsibility principle
- 1개의 class는 오직 1개의 역할만 가지고 있어야 한다.
- 만약에 class가 여러개의 역할을 가지면, 유지보수와 수정이 어려워 진다. 왜냐하면, 1개의 역할을 바꾸면, 다른 class들이 영향을 받기 때문이다.


## Open/Closed principle
- 1개의 class는 내부 수정에 관해서는 비공개 되어야 하고, extension에 대해서는 공개 되어야 한다.


## Liskov Principle
- parent class로 만든 객체는 sub class로 만든 객체로 대체가 가능해야한다.
- LSP를 violate 하면 Segregation principle을 violate 한다.

## Interface segregation principle
- 1개의 class는 사용하지 않는 interface와 method들을 implement 하지 않아도 되게 만들어야 한다.
- Interface는 최대한 작고, 목적 집약적으로 작성해야 한다.

## Dependency inversion principle
- parent 단계의 module 파일은 하위 단계의 module에 의존하면 안된다.
---
# INVEST

## Independent
- Each user story should be independent of others, so that it can be implemented and tested without dependencies on other stories.

## Negotiable
- User stories should be open to discussion and negotiation between the development team and stakeholders, in order to ensure that they are realistic and achievable.

## Valuable
- Each user story should provide value to the user or customer, and help to achieve the overall goals of the project.

## Estimable
- User stories should be small enough to be easily estimated by the development team, in terms of time, effort, and resources required.

## Small
- User stories should be small enough to be implemented and tested within a single development cycle, typically one or two weeks.

## Testable
- User stories should be testable, with well-defined acceptance criteria that can be used to verify that the story has been implemented correctly.

___
# Coverage testing
- Coverage testing은 작성한 테스트 파일에서 source 코드중 몇퍼센트가 사용되는지를 측정하는 테스트이다.
- Test들이 소프트웨어를 잘 test하는지를 측정하기 위해 만든 테스트이다.
- Coverage test는 코드의 정확도를 측정하지 않는다.
- Unit test와 같이 간편하게 소프트웨어의 성능을 측정할수 있다.
- 개발자에서 직관적으로 성능을 보여준다.
- 단점은 input이 인위적이라서 모든 케이스를 고려하기 힘들다는 것이다.
- Coverage testing은 적은 컴퓨터 resource를 사용한다.

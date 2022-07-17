# Decorator Pattern

## 사용한 예시
### React Store -> UserStore
- https://github.com/gringrape/coding-life/pull/3

비즈니스 로직을 UserStore로 분리하였다.
UserStore에서 상태가 업데이트 될때마다 UI의 강제 업데이트를 일으키기 위해서해당 기능을 decorator 패턴을 이용해 분리해주었다. 

### TypeScript - Decorator
- https://www.typescriptlang.org/docs/handbook/decorators.html

## 위키 정의

> the decorator pattern is a design pattern that allows behavior to be added to an individual object, dynamically, without affecting the behavior of other objects from the same class.

특정 객체에 동작을 추가하는 패턴.

> The decorator pattern is often useful for adhering to the Single Responsibility Principle, as it allows functionality to be divided between classes with unique areas of concern.

추가되는 동작을 별도의 클래스로 분리할 수 있기 때문에, 관심사의 분리에 유리하다. 

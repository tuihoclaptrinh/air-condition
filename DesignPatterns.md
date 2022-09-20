# Design Patterns
## 1. Creational Patterns
- Abstract Factory
- Builder
- Factory Method
- Prototype
- **Singleton**: A class of which only a single instance can exist.
  - *Ex*: I want one class just have one and only one instance of this class in application.
  - Give private access modifier
  - *apply*:
  	1. Login : Save history user, action user(have 1 object log, and run anywhere I want, and data applicaition unaffected by log so it's safe).
  	2. Config: 1 application needed 1 collection config, so suggest singleton.
  	3. Caching: All application cache in one file.
  	4. Global resource
  - *problem*: Multi Threading
  - *Ex2*: TuihoclaptrinhSingleton:
    1. Private Constructor make sure that just have one tuihoclaptrinh.
    2. function public static getInstance: return one tuihoclaptrinh singleton.
    3. 2 to 3 ways to create singleton:
    4. Create directly: run application and run.
       - uni = new TuihoclaptrinhSingleton()
       - *problem*: first time I dont use this and lately I use it so it wasted resource.
       - *solve*: creating lazy loading: just create when I'm using.
         1. Check if null => new else return;
         2. *problem*: 
## 2. Structural Patterns
- Adapter
- Bridge
- Composite
- Decorator
- Facade
- Flyweight
- Proxy
## 3. Behavioral Patterns
- Chain of Resp.
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

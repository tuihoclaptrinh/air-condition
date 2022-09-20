# Design Patterns
## 1. Creational Patterns
- Abstract Factory
- Builder
- Factory Method
- Prototype
- Singleton
  - vd: co 1 class va chung ta chi muon co 1 va chi 1 instance cua class day trong application.
	- dua cho no 1 quyen truy cap toan cuc.
	- ung dung: . login
		+ Luu lai lich su user, action user (chi can 1 object log, va chay bat ki dau cta muon,
			va log ko anh huong den ung dung data nen xai an toan)
			 . config
		+ 1 ung dung chi can 1 collection config, nen xai singleton
			 . caching
		+ ca application cache ve 1 file
			 . Global Resource
	- problem: . ve viec multi threading
	- vidu TuihoclatrinhSingleton:
		+ private constructor dam bao chi co 1 tuihoclaptrinh tren doi thui
		+ ham public static getInstance: return 1 tuihoclaptrinh singleton
		+ co 2 - 3 cach tao ra singleton:
		_ Tao thang: bat app len la chay luon
			. uni = new TuihoclaptrinhSingleton()
			. problems: vd tg ko su dung r sau 1 khoang tg moi sd thi bi lang phi resource
			. solve: tao ra lazy loadding: chi khoi tao khi t su dung no
			. chay qua check neu null thi new con k thi return;
			. problems:  
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

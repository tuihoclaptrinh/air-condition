# Design Patterns
[Creational Patterns]

Abstract Factory	Creates an instance of several families of classes
Builder			Separates object construction from its representation
Factory Method		Creates an instance of several derived classes
Prototype			A fully initialized instance to be copied or cloned
Singleton			A class of which only a single instance can exist
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
------------------------------------------------------------------------------------------------------
Structural Patterns

Adapter			Match interfaces of different classes
Bridge			Separates an object’s interface from its implementation
Composite			A tree structure of simple and composite objects
Decorator			Add responsibilities to objects dynamically
Facade			A single class that represents an entire subsystem
Flyweight			A fine-grained instance used for efficient sharing
Proxy				An object representing another object
------------------------------------------------------------------------------------------------------
Behavioral Patterns

Chain of Resp.		A way of passing a request between a chain of objects
Command			Encapsulate a command request as an object
Interpreter		A way to include language elements in a program
Iterator			Sequentially access the elements of a collection
Mediator			Defines simplified communication between classes
Memento			Capture and restore an object's internal state
Observer			A way of notifying change to a number of classes
State				Alter an object's behavior when its state changes
Strategy			Encapsulates an algorithm inside a class
	- đưa imple ra ngoài, không liên quan đến object sử dụng.
	- object-oriented design is the "open-closed priciple"
	- khi thay doi, nang cap, extends, thi rat de de lam.
Template Method		Defer the exact steps of an algorithm to a subclass
Visitor			Defines a new operation to a class without change

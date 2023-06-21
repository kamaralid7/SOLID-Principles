# SOLID Principles

1.	S: Single Responsibility Principle (SRP)
2.	O: Open-closed Principle (OCP)
3.	L: Liskov substitution Principle (LSP)
4.	I: Interface Segregation Principle (ISP)
5.	D: Dependency Inversion Principle (DIP)

# Advantages of SOLID design principles in C#
1.	Maintainability
2.	Testability
3.	Flexibility and scalability
4.	Parallel development

# Open/Closed Principle
“Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification.”

Modules that follow the Open/Closed Principle include two key attributes.

##	Open for extension.
It means that the module’s behavior can be extended. 
When the requirements of the application change, you can extend the module with new behaviors that adapt to those changes.

##	Closed for modification.
The source code of such a module is inviolate when you extend the module's behavior. 
You shouldn't refactor and modify the existing code for the module until bugs are detected. 
The reason is the source code has already passed the unit testing, so changing it can affect other existing functionalities.

#	Liskov Substitution Principle
“You should be able to use any derived class instead of a parent class and have it behave in the same manner without modification.”

This principle clearly states that when you have a parent class and a child class in your project, 
the child class can be a substitution of the parent class without changing the correctness of the application.

#	Interface Segregation Principle
“Clients should not be forced to implement interfaces they don't use. 
Instead of one fat interface, many small interfaces are preferred based on groups of functions, each one serving one submodule.”


#	Dependency Inversion Principle
It’s the last principle in SOLID and states two critical parts as follows:

High-level modules should not depend on low-level modules. Both should depend on abstractions (interface).
Abstractions should not depend upon details. Details should depend on abstractions.
The high-level modules include the important policy decisions and business models of an application. 
If these modules depend on the lower-level details, changes to the lower-level modules can directly impact the higher-level ones, 
forcing them to change in turn. 
When building a real-time application, 
the critical point is always to keep the high-level module and low-level module loosely coupled as much as possible. 
It helps to protect the other class while you are making changes to any specific class. 
All in all, instead of a high-level module depending on a low-level module, both should depend on an abstraction.
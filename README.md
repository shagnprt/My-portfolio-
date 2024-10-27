C# Projects
there are some projects i made using C# and .NET Framework
Projets:
- Carinsurance
- Entity-Framework-Code-First-console-application
- Employee-Class
- IQuittable

Carinsurance
CarInsurance ASP.NET MVC ENTITY FRAMEWORK This project is an MVC web application that mimics a car insurance website. It takes the user's input on policy information and calculates a quote based on business logic. There is also an admin page that allows staff to view all of the quotes that have been issued

Entity-Framework-Code-First-console-application
Model Class (Student): Defines the structure of the database table.
DbContext (SchoolContext): Manages database connections and interactions.
Connection String: Specifies database details for EF to connect or create it.
Migrations: Automatically generated scripts to update database schema based on model changes.
CRUD Operations in Program.cs: Code for adding, reading, updating, and deleting Student records in the database.

Employee-Class
Employee Class: Contains properties Id, FirstName, and LastName.

Overloaded == Operator: This method checks if two Employee objects are equal by comparing their Id properties. If both objects are null, they are considered equal. If only one is null, they are not equal. If both are non-null, their Id properties are compared.

Overloaded != Operator: This is the opposite of the == operator, checking if two objects are not equal.

Override of Equals and GetHashCode: These methods are overridden to ensure that the logic of equality is consistent with the overloaded operators. Overriding GetHashCode() prevents warnings when comparing objects that overload == and !=.

Program Class: Two Employee objects, emp1 and emp2, are instantiated with different Id values, and they are compared using the overloaded == operator. Then, a third Employee object (emp3) with the same Id as emp1 is created, and emp1 is compared with emp3.

IQuittable
 Interface IQuittable: This interface defines a contract with a Quit() method that any class implementing the interface must provide. Employee Class: Inherits from IQuittable and implements the Quit() method. This method can be customized in any way (e.g., printing a message). Polymorphism: The object quittableEmployee is created with the type IQuittable but instantiated as an Employee. This demonstrates polymorphism because although the object is of type IQuittable, it uses the implementation of the Quit() method from the Employee class. Calling the Method: The Quit() method is called on the quittableEmployee object, and it runs the implementation defined in the Employee class.

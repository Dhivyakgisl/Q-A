**SAMPLE QUESTIONS RELATED TO BEAN**

1.  What is Bean?

Ans: The bean tag is a combination of the **set** and **push** tags, it allows
you create a new instance of an object and then set the values of the variables.
It then makes the bean available in the valuestack, so that it can be used in
the JSP page.

1.  What is Data Access Object (DAO) pattern in Java?

Ans: In short Data Access Object or DAO design pattern is way to reduce coupling
between Business logic and Persistence logic.DAO pattern allows you to
encapsulate code for performing CRUD operation against persistence from rest of
application. Which means any change on persistence logic will not affect other
layers of application which is already tested.

1.  What are the attributes of get and set methods in bean class?

Ans: A read-only attribute will have only a get**PropertyName**() method, and a
write-only attribute will have only a set**PropertyName**() method.

1.  What are the types of statements in JDBC?

Ans: JDBC API has 3 Interfaces and their key features of these are as follows:

**Statement:** which is used to run simple SQL statements like select and
update. Statement interfaces use for general-purpose access to your database. It
is useful when you are using static SQL statements at runtime. The Statement
interface cannot accept parameters.

**Prepared Statement:** A SQL statement is pre-compiled and stored in a Prepared
Statement object. It is used to run Pre compiled SQL. This object can then be
used to efficiently execute this statement multiple times. The object of
Prepared Statement class can be created using Connection.prepareStatement()
method. This extends Statement interface.

**Callable Statement:** This interface is used to execute the stored procedures.
This extends Prepared Statement interface. The object of Callable Statement
class can be created using Connection.prepareCall() method.

1.  Define MVC

Ans: MVC is a design pattern called Model-View-Controller. It decouples data
access logic from business logic.

1.  Define Model

Ans:The Model contains the core of the application's functionality. It
encapsulates the state of the application. Sometimes the only functionality it
contains is state. It knows nothing about the view or controller.

Example: Bean and DAO Class.

1.  Define view

Ans: The view provides the presentation of the model. It is the look and feel of
the application. The view can access the model getters, but it has no knowledge
of the setters. In addition, it knows nothing about the controller. The view
should be notified when changes to the model occur.

Example: Jsp,Html,Xml,etc..,

1.  Define controller

Ans: The controller reacts to the user input. It creates and sets the model and
helps to identify which view should be part of response.

Example: Action classes (struts)

1.  **What are Java Beans?**

**Ans:** Java Beans are usual Java classes which adhere to certain coding
conventions:  
Implements java.io.Serializable interface  
Provides no argument constructor  
Provides getter and setter methods for accessing it's properties.

1.  **Why do I get a NullPointerException when loading a JAR file into the
    BeanBox?**

Ans: Usually this is because of a mistake in the JAR file being loaded. In the
meantime, typical errors include:  
The MANIFEST file uses classes using the wrong file separator ("/" should be
used in all platforms).  
The MANIFEST file refers to classes in a package but the actual .class files are
not really in that package.

1.  **What is the serializable class in java beans?**  
    Any class is serializable as long as that class or a parent class implements
    the java.io.Serializable interface. Examples of serializable classes include
    Component, String, Date, Vector, and Hashtable.

2.  **What is the ActionForm?**

ActionForm is javabean which represents the form inputs containing the request
parameters from the View referencing the Action bean.

1.  **What are the important methods of ActionForm?**

The important methods of ActionForm are : validate() & reset().

1.  Define validate()

*validate()* : Used to validate properties after they have been populated;
Called before FormBean is handed to Action. Returns a collection of ActionError
as ActionErrors. Following is the method signature for the validate() method.

**public** ActionErrors validate(ActionMapping mapping,HttpServletRequest
request)

1.  Define reset()

reset() method is called by Struts Framework with each request that uses the
defined ActionForm. The purpose of this method is to reset all of the
ActionForm's data members prior to the new request values being set.

public void reset() {}

**What are the components of Struts Framework?**

Ans: Struts framework is comprised of following components:

1.  Java Servlets

2.  JSP (Java Server Pages)

3.  Custom Tags

4.  Message Resources

**What’s the role of a handler in MVC based applications?**

Ans:. It’s the job of handlers to transfer the requests to appropriate models as
they are bound to the model layer of MVC architecture. Handlers use mapping
information from configuration files for request transfer.

**What’s the flow of requests in Struts based applications?**

Ans: Struts based applications use MVC design pattern. The flow of requests is
as follows:

-   User interacts with View by clicking any link or by submitting any form.

-   Upon user’s interaction, the request is passed towards the controller.

-   Controller is responsible for passing the request to appropriate action.

-   Action is responsible for calling a function in Model which has all business
    logic implemented.

-   Response from the model layer is received back by the action which then
    passes it towards the view where user is able to see the response.

**Which file is used by controller to get mapping information for request
routing?**

Ans: Controller uses a configuration file “struts-config.xml file to get all
mapping information to decide which action to use for routing of user’s request.

**What’s the role of Action Class in Struts?** In Struts, Action Class acts as a
controller and performs following key tasks:

-   After receiving user request, it processes the user’s request.

-   Uses appropriate model and pulls data from model (if required).

-   Selects proper view to show the response to the user.

**How an actionForm bean is created?**

**Surrogate**

Ans: actionForm bean is created by extending the
class org.apache.struts.action.ActionForm

In the following example we have created an actionForm bean with the name
'testForm':

**. What are the two types of validations supported by Validator FrameWork?**

Ans: Validator Framework is used for form data validation. This framework
provides two types of validations:

1.  Client Side validation on user’s browser

2.  Server side validation

** What are the steps of Struts Installation?**

Ans: In order to use Struts framework, we only need to add Struts.Jar file in
our development environment. Once jar file is available in the CLASSPATH, we can
use the framework and develop Strut based applications.

**How client side validation is enabled on a JSP form?**

Ans: In order to enable client side validation in Struts, first we need to
enable validator plug-in in struts-config.xml file. This is done by adding
following configuration entries in this file:

Then Validation rules are defined in validation.xml file. If a form contains
email field and we want to enable client side validation for this field,
following code is added in validation.xml file: ** How action-mapping tag is
used for request forwarding in Struts configuration file?**

Ans: In Struts configuration file (struts-config.xml), forwarding options are
defined under action-mapping tag.

In the following example, when a user will click on the hyperlink **test.do**,
request will be forwarded to**/pages/testing.jsp **using following
configurations from struts-config.xml file:

** How duplicate form submission can be controlled in Struts?**

Ans: In Struts, action class provides two important methods which can be used to
avoid duplicate form submissions.

saveToken() method of action class generates a unique token and saves it in the
user’s session. isTokenValid() method is used then used to check uniqueness of
tokens.

**In Struts, how can we access Java beans and their properties?**

Ans: Bean Tag Library is a Struts library which can be used for accessing Java
beans.

**Which configuration file is used for storing JSP configuration information in
Struts?**

Ans: For JSP configuration details, Web.xml file is used.

**What’s the purpose of Execute method of action class?**

Ans: Execute method of action class is responsible for execution of business
logic. If any processing is required on the user’s request, it’s performed in
this method. This method returns actionForward object which routes the
application to appropriate page.

In the following example, execute method will return an object of actionForward
defined in struts-config.xml with the name “exampleAction”:

**What’s the difference between validation.xml and validator-rules.xml files in
Struts Validation framework?**

Ans: In Validation.xml, we define validation rules for any specific Java bean
while in validator-rules.xml file, standard and generic validation rules are
defined.

**How can we display all validation errors to user on JSP page?**

Ans: To display all validation errors based on the validation rules defined in
validation.xml file, we use \<html:errors /\> tag in our JSP file.

**What’s declarative exception handling in Struts?**

Ans: When logic for exception handling is defined in struts-config.xml or within
the action tag, it’s known as declarative exception handling in Struts.

**What’s DynaActionForm?**

Ans: DynaActionForm is a special type of actionForm class (sub-class of
ActionForm Class) that’s used for dynamically creating form beans. It uses
configuration files for form bean creation.

**What configuration changes are required to use Tiles in Struts?**

Ans: To create reusable components with Tiles framework, we need to add
following plugin definition code in struts-config.xml file:

**What’s the difference between Jakarta Struts and Apache Struts? Which one is
better to use?**

Ans: Both are same and there is no difference between them.

**. What’s the use of Struts.xml configuration file?**

Ans: Struts.xml file is one the key configuration files of Struts framework
which is used to define mapping between URL and action. When a user’s request is
received by the controller, controller uses mapping information from this file
to select appropriate action class.

**How tag libraries are defined in Struts?**

Ans: Tag libraries are defined in the configuration file (web.xml) inside
\<taglib\> tag as follows:

**\<taglib\>**

 

**\<taglib-uri\>/WEB-INF/struts-bean.tld\</taglib-uri\>**

 

**\<taglib-location\>/WEB-INF/struts-bean.tld\</taglib-location\>**

 

**\</taglib\>**

** What’s the significance of logic tags in Struts?**

Ans: Use of logic tags in Struts helps in writing a clean and efficient code at
presentation layer without use of scriptlets.

** What are the two scope types for formbeans?**

Ans: 1. Request Scope: Formbean values are available in the current request only

**How can we group related actions in one group in Struts?**

Ans: To group multiple related actions in one group, we can use DispatcherAction
class.

**When should we use SwtichAction?**

Ans: The best scenario to use SwitchAction class is when we have a modular
application with multiple modules working separately. Using SwitchAction class
we can switch from a resource in one module to another resource in some
different module of the application.

**What are the benefits of Struts framework?**

Ans: Struts is based on MVC and hence there is a good separation of different
layers in Struts which makes Struts applications development and customization
easy. Use of different configuration files makes Struts applications easily
configurable. Also, Struts is open source and hence, cost effective.

**What steps are required to for an application migration from Struts1 to
Struts2?**

Ans: Following Steps are required for Struts1 to Struts2 migration:

1.  Move Struts1 actionForm to Struts2 POJO.

2.  Convert Struts1 configuration file (struts-config.xml) to Struts2
    configuration file (struts.xml)

**How properties of a form are validated in Struts?**

Ans: For validation of populated properties, validate() method of ActionForm
class is used before handling the control of formbean to Action class.

**What’s the use of reset method of ActionForm class?**

Ans: reset method of actionForm class is used to clear the values of a form
before initiation of a new request.

** What are disadvantages of Struts?**

Ans: Although Struts have large number of advantages associated, it also
requires bigger learning curve and also reduces transparency in the development
process.

Struts also lack proper documentation and for many of its components, users are
unable to get proper online resources for help.

**. What’s the use of resourcebundle.properties file in Struts Validation
framework?**

Ans: resourcebundle.properties file is used to define specific error messages in
key value pairs for any possible errors that may occur in the code.

This approach helps to keep the code clean as developer doesn’t need to embed
all error messages inside code.

**. Can I have html form property without associated getter and setter formbean
methods?**

Ans: For each html form property, getter and setter methods in the formbean must
be defined otherwise application results in an error.

**How many servlet controllers are used in a Struts Application?**

Ans: Struts framework works on the concept of centralized control approach and
the whole application is controlled by a single servlet controller. Hence, we
require only one servlet controller in a servlet application.

**Which model components are supported by Struts?**

Ans: Struts support all types of models including Java beans, EJB, CORBA.
However, Struts doesn’t have any in-built support for any specific model and
it’s the developer’s choice to opt for any model.

**When it’s useful to use IncludeAction?**

Ans: IncludeAction is action class provided by Struts which is useful when an
integration is required between Struts and Servlet based application.

**Is Struts thread safe?**

Ans: Yes Struts are thread safe. In Struts, a new servlet object is not required
to handle each request; rather a new thread of action class object is used for
each new request.

**What configuration changes are required to use resource files in Struts?**

Ans:  Resource files (.properties files) can be used in Struts by adding
following configuration entry in struts-config.xml file:

\<message-resources parameter=”com.login.struts.ApplicationResources”/\>

**How nested beans can be used in Struts applications?**

Ans: Struts provide a separate tag library (Nested Tag Library) for this
purpose. Using this library, we can nest the beans in any Struts based
application.

**What are the Core classes of Struts Framework?**

Ans: Following are the core classes provided by Struts Framework:

-   Action Class

-   ActionForm Class

-   ActionMapping Class

-   ActionForward Class

-   ActionServlet Class

**Is Struts Framework part of J2EE?**

Ans: Although Struts framework is based on J2EE technologies like JSP, Java
Beans, Servlets etc but it’s not a part of J2EE standards.

**When should be opt for Struts Framework?**

Ans: Struts should be used when any or some of the following conditions are
true:

-   A highly robust enterprise level application development is required.

-   A reusable, highly configurable application is required.

-   A loosely coupled, MVC based application is required with clear segregation
    of different layers.

**Why ActionServlet is singleton in Struts?**

Ans: In Struts framework, actionServlet acts as a controller and all the
requests made by users are controlled by this controller. ActionServlet is based
on singleton design patter as only one object needs to be created for this
controller class. Multiple threads are created later for each user request.

** What are the steps required for setting up validator framework in Struts?**

Ans: Following Steps are required to setup validator framework in Struts:
– *Wrong Spelling*

1.  In WEB-INF directory place valdator-rules.xml and validation.xml files.

2.  Enable validation plugin in struts-config.xml files by adding following:

**Which technologies can be used at View Layer in Struts?**

Ans: In Struts, we can use any of the following technologies in view layer:

-   JSP

-   HTML

-   XML/XSLT

-   WML Files

-   Velocity Templates

-   Servlets

**What are the conditions for actionForm to work correctly?**

Ans: ActionForm must fulfill following conditions to work correctly:

-   It must have a no argument constructor.

-   It should have public getter and setter methods for all its properties.

**Which library is provided by Struts for form elements like check boxes, text
boxes etc?**

Ans: Struts provide HTML Tags library which can be used for adding form elements
like text fields, text boxes, radio buttons etc.

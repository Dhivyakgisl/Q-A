##### 1.Explain the core classes of the Struts Framework.

Answer:The core classes of Struts framework are:  
ActionServlet, ActionForm, Action, Action Mapping, ActionForward  
2**.**[What are the drawbacks of
Struts?](http://www.careerride.com/Struts-drawbacks.aspx)

answer:Drawbacks of Struts:

-   No backward flow

-   Single controller servlet – Only one ActionServlet is available which may be
    an issue of scalability.........

##### 3.Explain Struts navigation flow.

answer:When an action servlet gets the request, it initiates the
servlet-config.xml  
It selects an appropriate page as per the mapping...

##### 4.Explain the design patterns used in Struts.

answer:The Struts design pattern has N-tier architecture. This includes MVC
architecture, Web applications characters, struts framework which includes –
architecture, design patterns and coding idioms..  
5**.Explain the different kinds of actions in Struts.**

answer:The different kinds of actions are done by the following:  
DispatchAction, ActionDispatcher , LookupDispatchAction...  
6**.**[What is Action
Class?](http://www.careerride.com/Struts-what-is-action-class.aspx)

answer:This class is extended by the org.apache.struts.action.Action class. The
business logic is wrapped by the Action class and this class provides an
interface to the Model of the application  
7**.**[What is
ActionForm?](http://www.careerride.com/Struts-what-is-ActionForm.aspx)

answer:ActionForm is a Java bean that associates one or more ActionMappings. The
bean is initialized from the corresponding parameters of requests well before
the Action.execute method is invoked.  
8**.Describe the main difference between Action and DispatchAction classes.**

answer:Grouping related actions into one class is possible using DispatchAction
class. But in Action class a group related action into one class is not
possible..Several changes need to be done, when one plans to group the related
action using Action class..  
9**.What is switch action & forwardAction in struts?**

answer:A SwitchAction is like an Action which switches between modules and
forwards the control to the URI that is specified in the new module.  
10**.What is LookupDispatch Action?**

answer:LookupDispatch is similar to ActionDispatch. It distinguishes the
ActionDispatch that uses the request parameter’s values which performs a reverse
lookup from resource bundle which uses the value of parameters and match it to a
method in the class...

##### 11.Explain the difference between ForwardAction and IncludeAction.

answer:Forwarding to a specified URL is provided by the ForwardAction. The
mechanism to include the specified URL contents is proveided by the
IncludeAction  
12**.**[Explain the difference between Html tags and Struts specific HTML
Tags.](http://www.careerride.com/Struts-specific-HTML-tags.aspx)

answer:HTML tags are static and Struts tags are dynamic.  
Struts tags can be created by the page authors.  
13**.What are the contents of web.xml and struts-config.xml? Explain the
difference between them.**

answer:The web.xml file contains the information that is used by servlets and
JSPs. The file includes the description of the application, information about
servlets, mapping information for servlets and URL, JSP configuration
information....  
14**.**[Differences between web.xml and
sturts-config.xml](http://www.careerride.com/Struts-web.xml-and-sturts-config.xm.aspx)

answer:web.xml is utilized to make connections between web application and the
web container, where as the struts-config.xml is utilized to establish the
connections between the controller and the view of MVC architecture..

##### 15.Explain how to communicate from struts to ejb.

answer:The Struts framework strictly implements MVC pattern. The execute()
method of Action class can be invoked to interact with the Model part of MVC. An
EJB may contain a model. The model methods can be invoked by the execute()
method.  
16**.Define Struts.**

answer:Struts is a framework for creating Java web applications. Web
applications differ from conventional websites in that web applications can
create a dynamic response. Due to the blend of database, design and control flow
codes of JSP, the larger applications become difficult to maintain..  
17**.What are action form classes in Struts?**

answer:The Action is part of the controller. Action Class is used to translate
the HttpServletRequest to the business logic. To do this we need to overwrite
the execute() method...  
18**.**[What is
ActionServlet?](http://www.careerride.com/Struts-ActionServlet.aspx)

answer:It is a class in org.apache.struts.action. It plays the role of a
controller in the Jakarta Struts Framework..........  
19**.**[What is Struts Validator
Framework?](http://www.careerride.com/Struts-Validator-Framework.aspx)

answer:The validation of data, whether on the Client side browser form or on the
server side, can be done with the help of Struts Validator Framework..

##### 20.Explain directory structure for a struts folder.

answer:META-INF: Contains meta information. Used by utilities etc.  
WEB-INF/classes: This is where you place you own Java classes.  
WEB-INF/classes/ApplicationResources.properties: Contains the messages (fixed
texts) of the application. Error messages are also put here.

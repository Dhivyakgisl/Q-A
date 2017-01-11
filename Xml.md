*web.xml (Struts)*

\* *Note* : Web.xml is also known as Deployment Descriptor, Front Controller...

**Q1 :** What is web.xml?

>   **A1 :** - web.xml** **is used to control many facets of a Web application.

>   \- Through Deployment Descriptor file, web.xml, you can control many aspects
>   of the Web application behavior, from preloading servlets, to restricting
>   resource access, to controlling session time-outs.

#### Q2 : What is Deployment Descriptor?

#### A2 : - DD is a XML document with .xml extension. 

#### \- describes the deployment settings of an application or module or the component.

#### \- At runtime, server reads the DD and understands it, then acts upon the information mentioned in descriptor.

**Q3 :** Abbreviate xmlns:xsi, xmlns.

**A3 :** Xmlns:xsi xml namespace: xmlschema instan

Xmlns xml namespace

Q4 : What if there is no welcome-file-list element in web.xml?
==============================================================

**A4 :** Just a HTTP 404 error page will be display.

**Q5 :** Describe welcome-file element.

**A5 :** It represent .jsp/.html file to be executed at first.

Q6 : “ \*.do ” in web.xml file ?
================================

>   **A6 :** Servlet-Mapping is useful in hidding your real servlet class names
>   by simple adding the \*.do as mapping the user cannot know which servlet it
>   is pointing to.

**Q7 :** What is load-on-startup?

>   **A7 :** It tells the web container about loading a particular servlet. It
>   is Mandatory.  
>   Remember lower the value of \<load-on-startup\>, servlet will be loaded
>   first.

*struts-config.xml*

**Q8 :** What is struct-config.xml?

**A8 : -** It is struts configuration file.

-   Configure the controller and view pages.

**Q9 :** What is Forward?

**A9 :** A forward can be local for specific action. A local forward is defined
in a struts-config.xml file in an action mapping and is invoked when the action
is invoked.

**Q10 :** What is global-forwards?

>   **A10 :** global-forwards available to any action. It is defined in a
>   struts-config.xml file in action-mapping.

Choose from the Options.

\**Note* : *DD* represents *D*eployment *D*escriptor.\*

Q1 : Which of these is true about deployment descriptors ?. Select the correct
answer.

Options :

1.  The order of elements in DD is not important.

2.  The elements of DD are case insensitive.

3.  The servlet-mapping element, if defined, must be included within the servlet
    element.

4.  The web-app element must include the servlet element.

>   A : 1. In the DD the elements in the web-app element can come in any order.

Q2 : Which of these files is the correct name and location od DD of a web
application ?.

Options :

1.  \\doc-root\\dd.xml

2.  \\doc-root\\WEB-INF\\dd.xml

3.  \\doc-root\\WEB-INF\\web.xml

4.  \\doc-root\\WEB\_INF\\web.xml

5.  \\doc-root\\WEB\_INF\\dd.xml

6.  \\doc-root\\WEB-INF\\lib\\web.xml

>   A : 3. \\doc-root\\WEB-INF\\web.xml

Q3 : The exception-type element specifies an exception type and is used to
handle exceptions generated from servlet. Which element of the DD includes the
exception-type as a sub-element.

Options :

1.  error-page

2.  servlet

3.  exception

4.  error-handling

>   A : 1. error-page

Q4 : Which element of the DD of a web application includes the welcome-file-list
element as a subelement.

Options :

1.  web-app

2.  welcome-file

3.  servlet

4.  file-list

>   A : 1. Web-app

Q5 : The root of the DD is named as

Options :

1.  web

2.  web-app

3.  name

4.  display name

>   A : 2. web-app

## HTML
### Form
#### Whenever you want to collect information from visitors you will need a form, which lives inside a **form** element.
#### Information from a form is sent in name/value pairs .
##### Example 
`<input type="search" name="search" />`
#### Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
#### The <label> element can be used in two ways. It can :
##### 1. Wrap around both the text description and the form input .
##### 2. Be kept separate from the form control

#### HTML5 introduces new form elements which make it easier for visitors to fill in forms

#### The **button** element was introduced to allow users more control over how their buttons appear .
` <button><img src="images/add.gif" alt="add" width="10" height="10" />`

#### **select** A drop down list box it have option element inside it

![Form](https://th.bing.com/th/id/R7a7052d9e950c017b3e6c42365e2d5ca?rik=bZx4Di7CZzCe1A&riu=http%3a%2f%2fwww.htmlgoodies.com%2fimg%2f2010%2f06%2fHTML-Forms-From-Basics-to-Style-Layouts-Figure2.gif&ehk=z7Oti8WdBTSR3ejzXi21JatQEpb19820X7AtIYuDOnE%3d&risl=&pid=ImgRaw)


### List , Table and Forms
#### List markers can be given different appearances using the list-style-type and list-style image properties

#### Table cells can have different borders and spacing in  different browsers, but there are properties you can use to control them and make them more consistent. 


#### The **table** element is used to add tables to a web page.

#### A table is drawn out row by row. Each row is created with the *tr* element.
#### Inside each row there are a number of cells represented by the *td* element (or *th* if it is a header) .
#### You can make cells of a table span more than one row or column using the rowspan and colspan attributes.
#### For long tables you can split the table into a *thead*, *tbody*, and *tfoot* .
![Table](https://a.ilovecoding.org/img/table-all-about-creating-simple-to-complex-html-tables-sc18.png)

#### There are three types of HTML lists: 
##### 1. orderd 
##### 2. unorderd
##### 3. definition

#### Ordered lists use numbers
`<ol><li>list item</li></ol>`
#### Unordered lists use bullets
`<ul><li>list item</li></ul>`
#### Definition lists are used to define terminology
`<dl><dt>list item</dt></dl>`
*( dt ) contain the term being defined and ( dd ) is used to contain the definition.*
#### Lists can be nested inside one another.


## JavaScript
### Events
#### Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
#### Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon. 
#### When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
#### You can use event delegation to monitor for events that happen on all of the children of an element.
![Events](https://cdn.javascripttutorial.net/wp-content/uploads/2019/12/javascript-event-loop-step-2.png)
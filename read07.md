## Domain Modeling
#### Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.
#### To define the same properties between many objects, you'll want to use a constructor function.
##### Here's an implementation of the EpicFailVideo constructor function.
###### var EpicFailVideo = function(epicRating, hasAnimals) {this.epicRating = epicRating; this.hasAnimals = hasAnimals; } 

#### To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function.


## HTML 
### Tables
#### The **table** element is used to add tables to a web page.
#### A table is drawn out row by row. Each row is created with the *tr* element.
#### Inside each row there are a number of cells represented by the *td* element (or *th* if it is a header) .
#### You can make cells of a table span more than one row or column using the rowspan and colspan attributes.
#### For long tables you can split the table into a *thead*, *tbody*, and *tfoot* .
![Table](https://a.ilovecoding.org/img/table-all-about-creating-simple-to-complex-html-tables-sc18.png)


## JavaScript
### Functions, Methods, and Objects
#### Functions let you group a series of statements together to perform a  specific task. If different parts of a script repeat the same task, you can  reuse the function (rather than repeating the same set of statements). 
##### Example : 
##### *function updateMessage() {var el = document.getElementByld('message'}; el .textContent = msg;*

![Function component](https://res.cloudinary.com/practicaldev/image/fetch/s--OKK_5-yp--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://raddevon.com/wp-content/uploads/2019/07/function-declaration-diagram-1024x282.png)

##### xample of calling a function :
`sayHello();`
##### if it has an information :
`sayHello('Width','height');`

#### Functions allow you to group a set of related statements together that represent a single task. 
#### Functions can take parameters (informatiorJ required to do their job) and may return a value.
###### function('String',Number){any thing you want}

#### An object is a series of variables and functions that represent something from the world around you.
##### Example of object:
`let variables = {'first':10 , 'second':20} ` 
#### In an object, variables are known as properties of the object; functions are known as methods of the object. 
#### Web browsers implement objects that represent both the browser window and the document loaded into the browser window. 

#### JavaScript also has several built-in objects such as :
##### 1. String
##### 2. Number 
##### 3. Math
##### 4. Date

#### Arrays and objects can be used to create complex data sets .
###### {accom: 460, food: 20, phone: 20} 
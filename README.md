# T3A1 - Workbook




#### Q1	Provide an overview and description of a standard source control process for a large project

---
A large project should implement the use of a version control system to manage and track changes over the project lifetime. Using Git as an example, a team would start by setting up a remote centralized repository that all members can access. GitHub, GitLab or bitbucket are all common examples of platforms that can host this code for all users to access.

The next steps has team members pull down a copy of this repository to their local machines threw a process known as cloning. they then logout of the main branch onto a newly created side branch to work on the component assigned. Typically the branch name describes the modifications taking place. this will allow them to work independently without affecting the main code. They should perform regular meaningful commits to aid in code review and less destruction when reverting changes.

All code pushed to the remote repository typically presents a pull request to be merged into the main project. Another team member that did not work on the code will then review the code to ensure quality and adhere to any coding standards of the project.

Documentation that outlines processes used, branching stategies employed and other relavant information should be maintained for quick onboarding of new team members and consistancy in colloboration with the project.

---
#### Q2	What are the most important aspects of quality software?
---
Functionality - The software need to meet the requirements of the users providing features that compliment the user experience. It needs to do this both efficienty and accurately. Taking a web browser as an example features such as the addition of tabs, bookmarking sites and web extensions all add functionality while still maintaining a smooth and responsive browsing experience.

Reliability - Having a robust platform that not only dependable but consistant and predictable in it's behaviour. This includes it's ability to handle errors gracefully. We expect that a web browser would work on many different hardware setups. That when the internet is down it will provide us with the same message and point us in the direction of how to fix the problem. That when we log back in the bookmarks that are saved should still be there.

Usability - Needs to be user-friendly. This could include intuitive interfaces, clear instruction and efficient workflows. Accessabilty for disabilities, keyboard shortcuts etc also add to the usability of an application. A good example of usability might be a search bar being shown on shopping website that when people use it will find things with the key word search.

Efficiency - The use of system resources should be kept to a minimum and avoid wasted computational power in performing a task while also being fast. Efficient programs properly balance these two aspects. To improve efficiency many underlying techniques can be used such as improving the algoririthm complexity, caching, compiling code or multithreading as well as choosing the correct programming language or databasing methodoligy. The V8 engine which runs in google chrome for example creates efficiency by compiling javascript into machine code improving web application excecution speed.

Security - People want their data protected from unauthorized access. Good software implementation uses encryption, authentication and authorization to safeguard sensitive data as well as maintain the integrity of it. With cyber criminals adapting to global change so too does the security implementations being used. Logging into a government website might take not only a password but a securely sent text message with a number of digits.

Maintainability - Is the software structure well designed and easy to adapt? we want to see DRY, modular code alongside well written documentation. This will make any updates, enhancements, bug fixes alot easier to apply. This is crucial to ensuring the longevity of a product. Many frameworks for building applications provide architucture models to help with maintainability. For example developers of Flask applications often adopt an MTV (model-template-view) archetecture by convention to improve the maintainablity of the code. 

---
#### Q3	Outline a standard high level structure for a MERN stack application and explain the components
---
The acrynym MERN stands for MongoDB, Express.js, React, Node.js.

MongoDB is noSQL database management system that serves to hold the persistant data of the application. Express.js is the framework that is used to simplify the process of building an API that will connect to this database. Node.js is the environment that executes all of the JavaScript on the server side handling all the logic, routing and interactions with the database. React is used to build our front-end that will communicate with the API built by Express.js and the rest of the backend logic. 

1. project root
* app.js - entry point. sets up all of the connections and defines the routes.
* package.json - lists dependancies of the code, commands, name, licensing etc.
* .env - houses all of the environement variables including database connection strings, API's and security keys
2. Backend - Epress.js & Node.js
* config
*controllers
*routes
*models
3. Frontend - React
* components
* 

4. Database - MongoDB
* cluster and database setup
* models

---
#### Q4	A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?
---
Depending on the scale and goals of the small business it might be best to opt into a website building solution. If we are looking for scalability and custom solution however an understanding of Web development languages is where we should start. This includes but both HTML and CSS which are fundemental for structuring and styling web pages as well as Javascript for adding interactivity.  Alongside these basics it would be important to gain a solid understanding of the following,

1. Version Control - This is so the team can work collaboratively and track changes to the project. One of the most prominent forms of version control being GIT and the basics should be atleast developed.   
2. A frontend Framework/Library - Depending on what the business is looking for in terms of responsiveness and user interface. There are a range of options of the market including React, Angular, Vue.js.
3. Backend and developement - Select a backend technology that is suitable for the team. Node.js pair well with React for example. Others such as Flask or Ruby on Rails could be viable options but would require learning additional programming languages. 
4. server-Side development - knowledge of server-side frameworks i.e. Express.js,Django,Flask. This is to handle any HTTP requests, business logic etc.
5. Database management - Understanding of how databases store data and how to retrieve that data.
6. Web API's - knowledge of how to interact and build API's.
6. An understanding of Websecurity - how to build and design your site so that it can be safe from cyber attacks as well as maintain integrity of user/client data.
7. Deployment and Webhosting - the understanding of how to deploy the website for others to access. Common hosting sites.
8. Testing - knowledge of how to test and use testing tools eg. Jest to ensure the website is working accordingly
9. Documentation
10. A skillset in troubleshooting and adaptabilty to come up with solutions to problems.

Alongside these fundemental concepts of programming the team should also develop skills in communication, project management and a little graphic design where needed. Learning and applying agile methodoligy to the build would also help to streamline the process. 

---
#### Q5	With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges
---
The Project I will mention is the T1A3. I build a Stocktake terminal application

1. Project management, and methodololigy
In term 1 I was tasked to build a terminal application. To even begin the project I needed to understand basic development patterns (agile methodoligy) and use a project management tool. I opted for Trello and layed out the project into tasks for completion. 
2. Git version control and record keeping
After laying out the general direction of the project I setup a remote repository on github and started pushed the local code that I started with to it. This was to start a pattern of recordkeeping.
3. WSL - Ubuntu
Considering the application was for the terminal it was important to gather an understanding of terminal commands. In my case bash commands to move around and create folders etc. This was made easier with the use of visual studio code. 
4. Shell scripting, virtual environment
I wrote a shell script to initialize the application so I had to gain the knowledge what a shell script was as well as the commands to achieve what I needed. The purpose of the shell script was to create a virtual environment and start the application, so I had to understand the why that was important as well as how different versions of software could affect the working of the application. As well as how packages would be installed inside of the virtual environment to keep it consistant across machines using the application. 
5. Javascript
The core of the program was written in python so I needed to learn that. 
- Functions, how to make my own as well as what inbuilt functions and methods already existed in python.
- Control flow. The main loop hold the menu which would access different parts of the program. Using logical operators, loops, if statements, try blocks etc. I was able to manipulate the flow of the program to suit the needs of the user.
- CSV and file manipulation - Rudementary understanding of document manipulation. This was touched on during classwork but I had to go to the internet/chatGPT to gain a better understanding of this to overcome the issue of data storage. 
- imports and package management
Need to understand what is available in the core of python that I could import direct and that which I needed to find and add. Also understand how to add and use and read documentation for implementing it. Tabulate is a example of this from outside core python used in my application.
- Styling - I wanted to implement different colours and styling so I also learnt a bit about ANSI escape codes. As well as the tabulate module to show the tables in nicer way.
- Improve user experience - I learnt about the time module to give users more time to read actions taking place before resetting the terminal. 
6. Documentation
The process of documenting all of the functionality of the program was a skillset needed to ensure that users understood the program and it's uses. I did this in the readme.md
7. Testing
I had to develop a strong testing mindset to make sure that all of the functionality that I was developing actually worked. Pytest was used to setup automated tests designed for core functionality but I also did quite a bit of manual testing.

---
#### Q6	With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature
---
Looking at the same T1A3 project. I believe my skillset on the onset of project was sufficient leaving enough room for me to grow and learn new things throughout. 

I would say I had a basic understanding of Project management, Git version control, WSL terminal commands, JavaScript but was lacking in testing and documentation processes.

---
#### Q7	Explain control flow, using an example from the JavaScript programming language
---
JavaScript is executed top to bottom. Control flow allow us to manipulate when and how many times these actions are taken. Using conditional statements, loops, function calling etc. are all goods ways of doing this. The code below uses a few of these different types of control structures to illistrate how the flow changes upon introduction of these tools.

```
function printWorld(activator) {
    // An if statement will change when a code runs based on whether the condition is true or false. 
    // If it's false it will proceed onto the next line without activation. 
    if (activator === "run") {

    // Loops will cause code to repeat itself. 
    // This for loop when activated prints Hello World to the console 5 times.
        for (i = 0; i < 5; i++) {
            console.log("Hello World")
        }
    } else {
            throw new Error("incorrect keyword used")
        }
}

printWorld("run") // A function like this one will tranfer the execution
                  // over to the functions pre-defined code and then return to this position once done.

```

---
#### Q8	Explain type coercion, using examples from the JavaScript programming language
---
Type coercion refers to the conversion of values from one data type to another. In particular JavaScript is known as loosely-typed meaning that variables can hold values of any data type and the intepreter will attempt to convert these values when involving other data types rather than immediately spiting out an erro. This is also known as implicit type conversion. Developers can als0 do this intentionally or explicitly. 

Example of implicit conversion
```
let i = 2; //data type: number
let j = "5"; //data type: string
let result = num + string; //coerces j from being a number to a string and concatenates
console.log(result) //output : "25" 

```
Example of explicit conversion
```
let i = 36; //data type: number
let j = "4" // data type: string
let result = Number(String) + num; //changes j from a string to a number and performs math addition
console.log(result) // output : 40

```
Due to implicit type conversion, JavaScript users may experience unexpected behaviour if they are not aware of how to handle the situation accordingly. For example Equality operators have two variants, ```==``` which allows implicit conversion and ```===``` which does not and this could product wildly different results under the right circumstances.

---
#### Q9	Explain data types, using examples from the JavaScript programming language
---
Data types are the type of value that is being used or being held by a variable. The data type is important for understanding how something is handled within the language. Lets look at the case of the following 2 code snippets ```let a = 2 + 2``` or ```let a = "2" + "2"```. The first shows 2 numbers that are added together and will result in a 4. The second takes two strings and concatenates them together to result in "22". Both look similiar but because the data type is different the "+" operator behaves differently creating different outcomes. JavaScript has a several different data types as follows; Numbers, Strings, Booleans, Undefined, Null, Symbols and Objects.

Numbers - unlike other languages Javascript only has one type of number stored in a 64-bit floating point. Integers are acurrate up to 15 digits and floating point arithmetic is not always accurate.
```
let Integer = 55
let FloatingPoint = 7.32
```
String - represent text and are stored between quotation marks
```
let greeting = "Sup, my Friend"
```
Boolean - logical operator with only two values of either true or false
```
let isTrue = true
let isFalse = false
```
Undefined - uninitialized or undefined value
```
let awesomeVariable;
console.log(awesomeVariable) // output: undefined
```
Null - intentional absence of value
```
let nullValue = null;
```
Symbol - A unique and immutable identifier
```
let uniqueSymbol = Symbol("unique")
```
Object - A collection of key-value pairs. key values are represented as strings where as values can be whatever datatype.
```
let petFish = {
  name: "Steven",
  species: "Black tetra",
  age: 5,
  isFood: false
}

```

---
#### Q10	Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language
---
Arrays can be manipulated using a variety of different built-in array methods that either add, remove or modify elements. To iterate over the array we would use a 'for of' loop or a generic for loop. There are also additional looping options in the array methods available that will manipulate the array. 

Add, Remove and Replace
```
let fish = ['Salmon', 'Tuna', 'Cod', 'Trout']

fish.push('Bass') // add to end of array
console.log(fish) // output: ['Salmon', 'Tuna', 'Cod', 'Trout', 'Bass']

fish.pop(); // removed from end of array
console.log(fish) // output: ['Salmon', 'Tuna', 'Cod', 'Trout']

fish.unshift('Carp') // add to beginning of the array
console.log(fish) // output: ['Carp', 'Salmon', 'Tuna', 'Cod', 'Trout']

fish.shift() // remove from beginning of the array
console.log(fish) // output: ['Salmon', 'Tuna', 'Cod', 'Trout']

fish.splice(1, 0, 'Angelfish') // add or remove elements as you define by the 3 parameters that are the index, how many elements to remove, what elements to add.
console.log(fish) // output: ['Salmon', 'Angelfish', 'Tuna', 'Cod', 'Trout']

fish.splice(1, 1, 'Pufferfish') // example of replacing a value using the splice method
console.log(fish) // ['Salmon', 'Pufferfish', 'Tuna', 'Cod', 'Trout']
```
Sorting, iterating and new arrays
```
let fish = ['Salmon', 'Tuna', 'Cod', 'Trout']
let favouriteFishIndex = fish.indexOf('Salmon') //finds the index of a value
let favouriteFish = fish.splice(favouriteFishIndex, favouriteFishIndex + 1) //cuts out a piece of the array as defined index positions
console.log(favouriteFish) // output: ['Salmon']

fish.sort(); //sorts the array alphebetically. note that for numerical sorting you will need to add a compare function as a parameter otherwise it will sort the values treating them as strings. eg. fish.sort((a,b) => return a - b) 
console.log(fish) // output: ['Cod', 'Trout', 'Tuna']
fish.reverse(); //reverses the sort
console.log(fish) // output: ['Tuna', 'Trout', 'Cod']

let prefix = 'big'
fish.forEach( (fishy) => { //iterate over each item in arrary and perform the function defined
  console.log(prefix + ' ' + fishy)
})

let newFishArray = fish.map((fishy) => prefix + ' ' + fishy) //creates a new array with the modifications of the callback function defined
console.log(newFishArray) 

for (newFish of newFishArray) { //iterates over the values of the array
  console.log(newFish)
}

for (i = 0; i < newFishArray.length; i++) { //iterates over each item of the array
  console.log(newFishArray[i])
}

```

---

#### Q11	Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language
---
Objects are a collection of key-value pairs. Keys are always strings but the values can be any datatype in the JavaScript programming language allowing us to modify what is set in those keys by using methods related to the specific data type. To access different values of the properties we can either use dot notation e.g. ```object.key``` or bracket notation ```object['key']```. Both point to value that relates to the key but it cirmcustances where special characters or spaces are in the key value you will have to use bracket notation. Examples of Object modification is as below.  

```
let car = {
  make: 'Toyota',
  model: 'Camry',
  year: 2022
};

car.colour = 'Red'; // adds a new property with the key colour and value 'Red'

delete car.year // removes the year property from car
```
To iterate over the properties of an object we can use the "for in' iterator
```
for (let key in car) { 
  console.log(`${key}: ${car[key]}`) //will print each property and key value pair to the console
}
```
Add your own method to the object using ```this``` keyword
```
car.name = function() { //adds the name key and function as a value to the car object
  return (this.make + " " + this.model) // this refers to the object it is applied to
} 
console.log(car.name())// output: 'Toyota Camry'


```
To check if a property exist we can use an if conditional
```
if ('brand' in car) {
  console.log('brand exists')
} else {
  console.log('brand does not exist')
} // output: brand does not exist 

```
objects are often associated with classes which act as templates to build objects following a set structure
```
class Car {
  constructor(make,model,year) {
    this.make = make
    this.model = model
    this.year = year
  }
}

newCar = new Car('Nissan', 'Navara', 1998) // makes a new object following the Car class template

```




---

#### Q12	Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language

---
To manipulate JSON we typically parse the data into a native JavaScript object and then apply changes using object methods. see Q11 answer for further details. 

When working with promises we are often receiving data in json format that we can covert quickly
```
response.json() //converts a received response from an API into a javascript object
```
But it's not always that simple and we may be required to convert it ourselves. This is where we need to use the built in JSON object and it's related methods to manipulate the data to the format we require.
```
let jsonString = '{
  "species": "Oak",
  "age": 50,
  "height": 20,
  "trunkDiameter": 1.2,
}

let tree = JSON.parse(jsonString); //converts JSON to a JavaScript object, you could modify the object using different object methods discussed in Q11.

tree.age = 51

let newJsonString = JSON.stringify(tree) //convert to a json string

```
Error handling when working with JSON is particularly critical as this is often user/external input into the code. We need to make sure that it is usable.
```
let invalidJsonString = '{"name": "Frank", "age": }'; //no age input making it invalid

try {
  let invalidObject = JSON.parse(invalidJsonString);
  console.log(invalidObject); // This won't be reached in case of an error
} catch (error) {
  console.error('Error parsing JSON:', error.message);
}
```





---

#### Q13	For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes
---

---

```
class Car { // initializes the class template for Car
  constructor(brand) { //special class method to build the object of the template. brand is a parameter that needs to be passed while initiaziling a new instance in future
    this.carname = brand; //this refers to the current object being constructed with carname as the key and brand as the value.
  }
  present() { // this is the creation of a class method
    return 'I have a ' + this.carname; // concatenates a string of with the brand taken from the initialization fo the object. whatever this method is applied to will be the object that this represents and will look for the key carname to return its value.
  }
}

class Model extends Car { //initialize a new class template taking elememnts from a the parent class of Car
  constructor(brand, mod) { // Same as earlier but takes an additional parameter called mod
    super(brand); //used to invoke the constructer of the parent class Car
    this.model = mod; //additional key-value specific to the Car class objectst that will be created.
  }
  show() { //another class method. this one is for the model class. will not work on the parent car class.
    return this.present() + ', it was made in ' + this.model; //returns a concatenated string of that invokes the parent class method present on the object to return the carname. it adds this to some words and then the model of value of the object is is called against.
  }
}

let makes = ["Ford", "Holden", "Toyota"] // An array of car brands. 
let models = Array.from(new Array(40), (x,i) => i + 1980)// Make a new Array 40 long without any values. From that array make another new array by iterating through each of the values adding the value of the index and 1980 to it. This creates a array of years ranging from 1980 to 2019 and stores it in models.

function randomIntFromInterval(min,max) { // min and max included // a function to determine a random interval. takes two parameters.
    return Math.floor(Math.random()*(max-min+1)+min); // 
}

for (model of models) {

  make = makes[randomIntFromInterval(0,makes.length-1)]
  model = models[randomIntFromInterval(0,makes.length-1)]

  mycar = new Model(make, model);
  console.log(mycar.show())
}
```
# T3A1 - Workbook




#### Q1	Provide an overview and description of a standard source control process for a large project

---
A large project should implement the use of a version control system to manage and track changes over the project lifespan. Using Git as an example, a team would start by setting up a remote centralized repository that all members can access. GitHub, GitLab or bitbucket are all common examples of platforms that can host code and be accessible to all members involved in the project.

The next steps have team members pull down a copy of this repository to their local machines in a process known as cloning. They then logout of the main branch onto a newly created side branch to work on a specific component assigned. Typically, the branch name describes the modifications taking place. By doing this they work independently without affecting the main code that they eventually sent back to hosting platform for review. They should perform regular meaningful commits to aid in the future code review. These commits should detail a note of exactly what was achieved.

All code pushed to the remote repository as a branch will then have pull request raised for it to be merged onto the main branch. Another team member that did not work on the code will then review it to ensure quality and adherence to any coding standards of the project. In the case of rejection notes will be added for the developer working on the branch to review. In the larger projects you may see someone assigned as a git master who primarily focuses on the code review aspects and the maintaining of the repository. Through the implementation of AGILE programming methodology there will be many iterations that need to be reviewed over the lifecycle of the project.

Before committing, during code review, after merging and before release are all important times to test the code to ensure that no issues arise.

Maintaining quality documentation that outlines processes used, branching strategies employed, and other relevant information will provide a solid foundation for on-boarding new team members and a point of reference for existing ones. This typically takes form of a README.md in the root directory of the project. It is also important to document version history and notes of changes to versions, licencing, acknowledgments etc.


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
The acronym MERN stands for MongoDB, Express.js, React, Node.js. Each are essentially pieces used to fill out the primary components of a full stack web application. The database, back-end and front-end.

MongoDB is noSQL database management system that serves to hold the persistent data of an application. It has good schema flexibility and most importantly, scalability. It stores information in compressed BSON files and they can be retrieved through the API in JSON format. It also supports integrated caching and is considered more user friendly. You would be connecting to this through an API built with Express.js and Node.js.
Express.js is a framework that is used to simplify the process of building an API. It's known to be robust, simple and provide middleware support making it well suited for HTTP requests. Important middleware included in the MERN stack are authentication and error handling functions that could end interaction if requirements aren't met. 
Node.js is the runtime environment that executes JavaScript code on the server side handling all the logic, routing, and interactions with the database. Its event driven, and has non-blocking in-out support, making running concurrent operations more efficient. 
React is used to build our front-end display for the user. It's component-based architecture promotes re-usability and maintainability in the code.

Below is the structure of a MERN stack application

1. project root
* app.js – is the entry point. Sets up all the connections and defines the routes.
* package.json - lists dependencies of the code, commands, name, licensing etc.
* .env - houses all of the environment variables including database connection strings, API's and security keys
2. Frontend – React
* components - reusable pieces of code built with react that are used across all the pages
* pages - Contains the components for entire pages
* App.js - Main component the coordinates the UI structure
* public – typically contains the HTML files and other static assets
* src – contains the index.js and index.css 
3. Backend and API structure - Epress.js & Node.js
* Config - configuration files for the application
* Controllers - responds to the HTTP requests and actions them
* Routes - defined pathways that the controllers use to access the database
* models - representation of the database structure 
4. Database - MongoDB
* Cluster and database setup - Mongo's setup for data storage
* Models - the defined structure in the MongoDB collections


---
#### Q4	A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?
---
Depending on the scale and goals of the small business it might be best to opt into a website building solution like wix. If we are looking for scalability and a custom solution however an understanding of Web development languages is where we should start. This includes but both HTML and CSS which are fundamental for structuring and styling web pages as well as JavaScript for adding interactivity.  Alongside these basics it would be important to gain a solid understanding of the following,

1. Version Control - This is so the team can work collaboratively and track changes to the project. One of the most prominent forms of version control being GIT and the basics should be at least developed.   
2. A frontend Framework/Library - Depending on what the business is looking for in terms of responsiveness and user interface. There are a range of options of the market including React, Angular, Vue.js. React for example streamlines front-end website creation using component structures and would be widely beneficial for team members to be familiar with.
3. Backend development - Select a backend technology that is suitable for the team. Node.js pair well with React for example. Others such as Flask or Ruby on Rails could be viable options but would require learning additional programming languages on-top of JavaScript. 
4. server-Side development - knowledge of server-side frameworks i.e. Express.js, Django, Flask. This is to handle any HTTP requests, business logic etc. The MDN web docs provide information on HTTP request methods as a good start.  
5. Database management - Understanding of how databases store data and how to retrieve that data. Also, the knowledge of different types of databases both SQL and noSQL to pick what is most suitable for your project. MongoDB, PostgreSQL as examples. A knowledge of how to write SQL queries as well.
6. Web API's - knowledge of how to interact and build API's and build them. Controllers, models, schemas etc.
6. An understanding of Web security - how to build and design your site so that it can be safe from cyber-attacks as well as maintain integrity of user/client data. Implementation of middleware and multi-step security techniques.
7. Deployment and Webhosting - the understanding of how to deploy the website for others to access. Common hosting sites like Netlify. 
8. Testing - knowledge of how to test and use testing tools e.g. Jest to ensure the website is working accordingly.
9. Documentation - Needed to ensure new team members joining know about the past iterations, how to use the website as well as how scalability is intended to happen.
10. A skillset in troubleshooting and adaptability to come up with solutions to problems.

Alongside these fundamental concepts of programming the team should also develop skills in communication, project management and a little graphic design where needed. Learning and applying agile methodology to the build would also help to streamline the process. 


---
#### Q5	With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges
---
The Project I will mention is the T1A3. I built a Stocktake terminal application

1. Project management
To begin the project I needed to understand basic development patterns (agile methodology) and use a project management tool. I opted for Trello and laid out the project into tasks for completion. 
2. Git version control and record keeping
After laying out the general direction of the project I setup a remote repository on GitHub and started pushed the local code that I started to it. I maintained consistent commitments as recordkeeping for each change and enhancement.
3. WSL - Ubuntu
Considering the application was for the terminal it was important to gather an understanding of terminal commands. In my case, bash commands to move around and create folders etc. This was made easier with the use of Visual Studio Code. 
4. Shell scripting, virtual environment
I wrote a shell script to initialize the application, so I had to gain the knowledge what a shell script was as well as the commands to achieve what I needed. The purpose of the shell script was to create a virtual environment and start the application within. I had to understand why that was important as well as how different versions of software could affect the working of the application. Also, how packages would be installed inside of the virtual environment. 
5. Python
The core of the program was written in python, so I needed to learn that. 
- Functions, how to make my own as well as what inbuilt functions and methods already existed in python.
- Control flow. The main loop for the menu which would access different parts of the program. Using logical operators, loops, if statements, try blocks etc. I was able to manipulate the flow of the program to suit the needs of the user.
- CSV and file manipulation - Rudimentary understanding of document manipulation. This was touched on during classwork, but I had to go to the internet/ChatGPT to gain a better understanding of this to overcome the issue of data storage. 
- imports and package management
Need to understand what is available in the core of python that I could import and use directly and that which I needed to find and add to assist with the program. Also understand how to read coding documentation to implement the functionality of the packages. Tabulate is an example of this from outside core python used in my application that I learnt.
- Styling - I wanted to implement different colours and styling so I also learnt a bit about ANSI escape codes. As well as the tabulate module to show the tables in nicer way.
- Improve user experience - I learnt about the time module to give users more time to read actions taking place before resetting the terminal. 
6. Documentation
The process of documenting all the functionality of the program was a skillset needed to ensure that users understood the program and it's uses. I did this in the readme.md toward the end of the project.
7. Testing
I had to develop a strong testing mindset to make sure that all the functionality that I implemented worked. Pytest was used to setup automated tests designed for core functionality, but I also did quite a bit of manual testing.


---
#### Q6	With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature
---
Many of the skills that I had during the time of developing my stocktake application were underdeveloped. Although that may have been the case, I believe the intended purpose was to develop the basics of what I had learnt during classwork. Let's review all of the skills above in Q5 and address how effective my knowledge was at the time of the T1A3 assignment.

1. Project management - A had the foundational knowledge to build the framework for project startup. Persistence to continually review progress throughout. Incorporate all the elements of the design into the tasks and add new tasks when time permitted to expanding the app. I estimated general completion times but failed to implement a good array of completion dates until later in the project, resulting in a scramble complete it. I would like to improve this in future by adding more dates on future cards. I also need to learn to use Trello more effectively for AGILE implementation. 

2. Version control - My understanding and implementation of git was sufficient to complete this project using add, commit, and push functions. Yet this was the bare minimum for the task. I would recommend being more comfortable with understanding each of the stages of the git process. Understanding and implementing group git methods as well as how to roll back versions using git could have saved me some time.

3. WSL - more than sufficient complete the job. I effectively could create and move around as needed. 

4. Shell scripting - my skillset was effective in building a script, executing a virtual environment, and cleaning it up after. There are a lot more versatile things that could have been implemented with shell scripting and learning more about the commands available would be beneficial. I would like to have a script setup to run tests exclusively for example. 

5. python - sufficient to start but required extensive growth and implementation throughout. Sometimes I implemented strategies that I was not quite familiar with resulting in global variables being used. I think having an understanding Big O notation and impacts of certain algorithms on performance would have helped to provide cleaner more efficient code. Better understanding of functions and how they interact with each other. A better grasp on functions could have resulted in writing more DRY code from the beginning.  

6. Documentation - lacking. I was not effective in providing upfront documentation nor had any experience reading or implementing it. I did however scrutinize and test the shell script to ensure that nothing was missed in the setup guide. Recommended to look over some documentation used by major publishers to getter a better idea for what would be needed and formats to use. Following the general pattern of others can make it easier for users to pick up the work that I have made.

---
#### Q7	Explain control flow, using an example from the JavaScript programming language
---
JavaScript is executed top to bottom. Control flow allow us to manipulate when, and how many times these actions are taken. Using conditional statements, loops, function calling etc. are all goods ways of doing this. The code below uses a few of these different types of control structures to illustrate how the flow changes upon introduction of these tools.

```
function printWorld(activator) {
    // An if statement will change when a code runs based on whether the condition is true or false. 
    // If it's false it will proceed onto the next line without activation. 
    if (activator === "run") {

    // Loops will cause code to repeat itself. 
    // This for loop when activated prints Hello World to the console 5 times. 
    // Alternatively the while loop exists that will run until a condition is no longer true.
        for (i = 0; i < 5; i++) {
            console.log("Hello World")
        }
    } else {
            throw new Error("incorrect keyword used")
        }
}

printWorld("run") // A function like this one will transfer the execution
                  // over to the functions pre-defined code and then return to this position once done.

```
Alternatively, to the if statements we could also use switch statements or ternary operators to achieve a similar result. Switches for large option pools and ternary operator for the 2 option only.
```
switch (day) { //switch statement. will look to see if the condition matches one of the cases and return that. It's more efficient than a large if statement.
    case 'Monday':
        console.log('It\'s Monday!');
        break;
    case 'Tuesday':
        console.log('It\'s Tuesday!');
        break;
    // ... other cases
    default:
        console.log('Not a valid day.');
}

function CanEnter(age) {
  return age < 18 ? "no, you are too young" : "yes, please come in" // ? is the ternary operator after it appears it will select either the left 
                                                                    // or right case depending on whether the condition is true or not.
}

```
In cases of error handling control flow is manipulated using the try-catch statement deflecting the code inside of the try block over to the catch code if any errors happen within.
```
try {
    isOld("45")
} catch (error) {
    throw new Error(error.message)
}

```



---
#### Q8	Explain type coercion, using examples from the JavaScript programming language
---
Type coercion refers to the conversion of values from one data type to another. JavaScript is known as loosely typed meaning that variables can hold values of any data type and the interpreter will attempt to convert these values when involving other data types rather than immediately returning an error. This is also known as implicit type conversion. Developers can also do this intentionally or explicitly. 

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
Due to implicit type conversion, JavaScript users may experience unexpected behaviour if they are not aware of how to handle the situation accordingly. For example Equality operators have two variants, ```==``` which allows implicit conversion and ```===``` which does not and this could produce wildly different results under the right circumstances.


---
#### Q9	Explain data types, using examples from the JavaScript programming language
---
"Data types" are the type of value that is being used or being held by a variable. The data type is important for understanding how something is handled within the language and how the runtime environment will treat it. Let's look at the case of the following 2 code snippets ```let a = 2 + 2``` or ```let a = "2" + "2"```. The first shows 2 numbers that are added together and will result in a 4. The second takes two strings and concatenates them together to result in "22". Both look similar but because the data type is different the "+" operator behaves differently creating different outcomes. JavaScript has several different data types as follows; Numbers, Strings, Booleans, Undefined, Null, Symbols and Objects.

Numbers - unlike other languages JavaScript only has one type of number stored in a 64-bit floating point. Integers are accurate up to 15 digits and floating point arithmetic is not always accurate.
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
Object - A collection of key-value pairs. key values are represented as strings where as values can be whatever datatype. This is also as a complex data type while the rest are all simple.
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
Arrays can be manipulated using a variety of different built-in array methods that either add, remove or modify elements. To iterate over an array we would use a 'for of' loop or a generic for loop. There are also additional looping options in the array methods available that will manipulate the array to be shown below. let's look at some examples, 

Add, Remove and Replace
```
let fish = ['Salmon', 'Tuna', 'Cod', 'Trout'] //initialize an array

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

fish.sort(); // sorts the array alphebetically. note that for numerical sorting you will need to add a compare function as a parameter 
             // otherwise it will sort the values treating them as strings. eg. fish.sort((a,b) => return a - b) 
console.log(fish) // output: ['Cod', 'Trout', 'Tuna']
fish.reverse(); //reverses the sort
console.log(fish) // output: ['Tuna', 'Trout', 'Cod']

let prefix = 'big'
fish.forEach( (fishy) => { //iterate over each item in array and perform the function defined
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
Objects are a collection of key-value pairs. Keys are always strings but the values can be any datatype in the JavaScript programming language allowing us to modify what is set in those keys by using methods related to the specific data types. To access different values of the properties we can either use dot notation e.g. ```object.key``` or bracket notation ```object['key']```. Both point to value that relates to the key but in cirmcumstances where special characters or spaces are used in the key, you will have to use bracket notation. Examples of Object modification is as below, 

```
let car = { //initilize an object inbetween {} with key-value pairs
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
Objects are often associated with classes which act as templates to build objects following the structures defined within
```
class Car {
  constructor(make,model,year) {
    this.make = make
    this.model = model
    this.year = year
  }
}

newCar1 = new Car('Nissan', 'Navara', 1998) // makes a new object following the Car class template

```




---

#### Q12	Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language

---
To manipulate JSON we typically parse the data into a native JavaScript object and then apply changes using object methods. see Q11 answer for further details. 

When working with promises we are often receiving data in json format that we can covert quickly.
```
response.json() //converts a received response from an API into a javascript object
```
But it's not always that simple and we may be required to convert it ourselves. This is where we need to use the built in JSON object and it's related methods to manipulate the data to the format we require.
```
let jsonString = '{ //initialize a json string 
  "species": "Oak",
  "age": 50,
  "height": 20,
  "trunkDiameter": 1.2,
}

let tree = JSON.parse(jsonString); //converts JSON to a JavaScript object, you could modify the object using different object methods discussed in Q11.

tree.age = 51 //adds age to the object

let newJsonString = JSON.stringify(tree) //convert back to a json string

```
Error handling when working with JSON is particularly critical as JSON is often user or external input. The most unpredictible and error prone type of data. We need to make sure that it is usable.
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
  constructor(brand) {    // special class method to build the object of the template. 
                          // Brand is a parameter that needs to be passed while initiaziling a new instance in future
    this.carname = brand; //this refers to the current object being constructed with carname as the key and brand as the value.
  }
  present() { // creation of a class method called present
    return 'I have a ' + this.carname;  // concatenates a string of with the brand taken from the initialization fo the object. 
                                        // whatever this method is applied to will be the object that this represents and will 
                                        // look for the key carname to return its value.
  }
}

class Model extends Car {               // initialize a new class template taking elements from a the parent class of Car
  constructor(brand, mod) {             // Another contructor but takes an additional parameter called mod
    super(brand);                       // used to invoke the constructer of the parent class Car
    this.model = mod;                   // additional key-value specific to the Car class objects that will be created.
  }
  show() {                              //another class method. this one is for the model class. will not work on the parent car class.
    return this.present() + ', it was made in ' + this.model; // returns a concatenated string of that invokes 
                                                              // the parent class method present on the object to return the carname. 
                                                              // it adds this some words and then the model value from the model object.
  }
}

let makes = ["Ford", "Holden", "Toyota"]                 // An array of car brands. 
let models = Array.from(new Array(40), (x,i) => i + 1980)// Make a new Array 40 long without any values. 
                                                         // From that array make another new array by iterating through each of the values 
                                                         // adding the value of the index and 1980 to it. This creates a array of years ranging
                                                         // from 1980 to 2019 and stores it in models. This is a range

function randomIntFromInterval(min,max) {                // a function to determine a random range. takes two parameters.
    return Math.floor(Math.random()*(max-min+1)+min);    //Randomizer, designed to return a value between 2 values given 
}

for (model of models) { // for loop that passes iterates over all of the values in the models array. 

  make = makes[randomIntFromInterval(0,makes.length-1)]   // applies our random function to the index of makes to return a random car 
                                                          // make and stores it in make
  model = models[randomIntFromInterval(0,makes.length-1)] //applies a random function to the index of models and stores it in model. 
                                                          // Note that is also alters the current iteration value because it shares the same name. 
                                                          // this will result in massive changes to the models array adding and removing year
                                                          // options for future cars in the cycle.

  mycar = new Model(make, model); // make a new object following the Model class template. uses the parameters defined earlier in the loop.
                                  // it's reassigned after each loop so early object iterations will be overwritten
  console.log(mycar.show())       // logs the return of the show method from class Model.  
}
```
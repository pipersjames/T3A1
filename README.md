# T3A1 - Workbook




#### Q1	Provide an overview and description of a standard source control process for a large project

A large project should implement the use of a version control system to manage and track changes over the project lifetime. Using Git as an example, a team would start by setting up a remote centralized repository that all members can access. GitHub, GitLab or bitbucket are all common examples of platforms that can host this code for all users to access.

The next steps has team members pull down a copy of this repository to their local machines threw a process known as cloning. they then logout of the main branch onto a newly created side branch to work on the component assigned. Typically the branch name describes the modifications taking place. this will allow them to work independently without affecting the main code. They should perform regular meaningful commits to aid in code review and less destruction when reverting changes.

All code pushed to the remote repository typically presents a pull request to be merged into the main project. Another team member that did not work on the code will then review the code to ensure quality and adhere to any coding standards of the project.

Documentation that outlines processes used, branching stategies employed and other relavant information should be maintained for quick onboarding of new team members and consistancy in colloboration with the project.






---

---
#### Q2	What are the most important aspects of quality software?



---

---
#### Q3	Outline a standard high level structure for a MERN stack application and explain the components



---

---
#### Q4	A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?


---

---

#### Q5	With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges


---

---

#### Q6	With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature

---

---


#### Q7	Explain control flow, using an example from the JavaScript programming language

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

---
#### Q8	Explain type coercion, using examples from the JavaScript programming language



---

---
#### Q9	Explain data types, using examples from the JavaScript programming language



---

---
#### Q10	Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language


---

---

#### Q11	Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language


---

---

#### Q12	Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language


---

---

#### Q13	For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes
---

---

```
class Car {
  constructor(brand) {
    this.carname = brand;
  }
  present() {
    return 'I have a ' + this.carname;
  }
}

class Model extends Car {
  constructor(brand, mod) {
    super(brand);
    this.model = mod;
  }
  show() {
    return this.present() + ', it was made in ' + this.model;
  }
}

let makes = ["Ford", "Holden", "Toyota"]
let models = Array.from(new Array(40), (x,i) => i + 1980)

function randomIntFromInterval(min,max) { // min and max included
    return Math.floor(Math.random()*(max-min+1)+min);
}

for (model of models) {

  make = makes[randomIntFromInterval(0,makes.length-1)]
  model = models[randomIntFromInterval(0,makes.length-1)]

  mycar = new Model(make, model);
  console.log(mycar.show())
}
```
## JavaScript Made Easy: Part 3

Hey there! and welcome back😊...If you are just coming in contact with this series, you can look up the previous topics I have discussed in JS here:
- [INTRODUCTION TO JAVASCRIPT](https://gracious-grace.hashnode.dev/introduction-to-javascript)
- [JAVASCRIPT MADE EASY: PART 2](https://gracious-grace.hashnode.dev/javascript-made-easy-part-2)

Today, I will be discussing the following topics in what manner? **An easy manner!**😊

- **JS let & const**
- **Conditional Statements**
- **JS Operators**

Without taking too much time, let's dive in immediately:

### JS LET & CONST

**LET**

- Like ```var```, the ```let``` keyword can also be used to declare variables, but, unlike ```var```, once you declare a variable using ```let```, the variable cannot be re-initialized or let me say you cannot declare another variable, using that same variable name unless it is re-initialized in a block scope e.g

```
var a=7
console.log(a) //7
//using the same variable name,a, to declare another variable
var a=8
console.log(a) //8

```
but unlike ```var```👇

```
let a=2
console.log(a) //2
let a=3
console.log(a) //error: variable 'a' has already been declared
{
let a=3 
console.log(a) //3
}
```
- ```let``` also enables block level scope, meaning, you can use the ```let``` keyword to declare variables you want to use in a particular block of code like a function or an object. 

```
{
    let a=3
    console.log(a) //3
    }
    console.log(a) //not defined
    

```

- ```let``` can be also used to stop hoisting. 

> Hoisting is a behavior in JS that allows variables to be used before they are declared. You can get a detailed explanation [here](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)

**CONST**

```const``` is used to declare variables whose value is not going to change once it has been declared..it is like a constant value e.g ```const PI=3.14```, but, in cases like objects, ```const``` values can be modified. 

```
const person = {
name1: "grace"
}
console.log(person.name1) // grace
person.name1="Young"
console.log(person.name1) //Young


```

### CONDITIONAL STATEMENTS

There are so many instances in a program where we want a specific block of code to run in a certain manner if it meets certain conditions. 

There are 3 types of conditional statements:

1.  **If-Else CONDITIONAL STATEMENT**
2. **If-Else if-Else CONDITIONAL STATEMENT**
3. **Switch case STATEMENT**

**Explanation:**

- **If-Else CONDITIONAL STATEMENT**

 We use the ```if``` ```else``` keywords when we have two possible outcomes(true or false) for an event.

```
//Syntax
if (condition1) {
    //if condition1 is true, write block of code to be executed here 
    }
else{
   //if conditonal one is false, write block of code to be executed here.
}

```

**Example:**

<iframe height="265" style="width: 100%;" scrolling="no" title="IfElseConditionalStatement" src="https://codepen.io/gra2101/embed/rNyzBoV?height=265&theme-id=dark&default-tab=js,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/gra2101/pen/rNyzBoV'>IfElseConditionalStatement</a> by Grace O.
  (<a href='https://codepen.io/gra2101'>@gra2101</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>


- **If-Else if-Else CONDITIONAL STATEMENT**

We use the ```if``` ```else if``` ```else``` keywords when we have three or more possible outcome for an event.

```
//Syntax
if (condition1) {
    // if condition1 is true, write block of code to be executed here 
    }
else if (conditional2) {
    // if conditional1 isn't true, write block of code to be executed here
   }
else{
   //if conditonal1 and condition2 are false, write block of code to be executed here.
}

```
**Example:**

<iframe height="265" style="width: 100%;" scrolling="no" title="If-Else if-Else" src="https://codepen.io/gra2101/embed/QWpMBQL?height=265&theme-id=dark&default-tab=js,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/gra2101/pen/QWpMBQL'>If-Else if-Else</a> by Grace O.
  (<a href='https://codepen.io/gra2101'>@gra2101</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

- **Switch case STATEMENT**

The JS ```switch``` statement is used to perform different actions based on different conditions. It is a good way to replace multiple ```else if``` statements. When the code starts executing, the value of the expression is compared with the values of each case. If there is a match, the associated block of code is executed. If there is no match, the default code block is executed. Look at a basic syntax we have below:

```
switch (expression) {
case a:
//code to be executed
break;
case b:
//code to be executed
break;
case c:
//code to be executed
break;
default:
//code to be executed
}

```


**Example: **

<iframe height="265" style="width: 100%;" scrolling="no" title="switch case" src="https://codepen.io/gra2101/embed/bGqrmOj?height=265&theme-id=dark&default-tab=css,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/gra2101/pen/bGqrmOj'>switch case</a> by Grace O.
  (<a href='https://codepen.io/gra2101'>@gra2101</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>


### JS OPERATORS

Under JS operators, we have:

- Unary operators
- Assignment operators
- Arithmetic operators
- String operator
- Shift operators
- Comparison operators
- Bitwise operators
- Logical operators
- Ternary operators
- Type operators

**UNARY OPERATORS**

The increment operator ```++``` increments (adds one to) its operand and returns a value and the decrement operator ```--``` decrements (subtracts one from) its operand and returns a value.

Unary operators can be **postfix** or **prefix** operator.

**Postfix:** meaning the operator comes after the operand ```a++```. It first assign before incrementing e.g

```
var a=2
console.log(a++) // 2
// or
console.log(a--) // 2

```
**Prefix:** meaning the operator comes before the operand ```++a```. It first increment, then assign.

Here is a postfix example:

```
var a = 2
console.log(++a) //3
// or
console.log(--a) //1

```

**ASSIGNMENT OPERATORS**

The assignment operator ```=``` is used to assign a value to a variable.
e.g

```
var a = 2
//a - variable
//2 - value

```

**ARITHMETIC OPERATORS**

The arithmetic operators comprises of all mathematical operators like add, subtract, multiply, divide, exponential, modulus.
e.g 
```
var a=10,b=5
//addition operator
console.log(a+b) //15
//subtraction operator
console.log(a-b) //5
//multiplication operator
console.log(a*b) //50
//division operator
console.log(a/b) //2
//exponential operator
console.log(a**b) // 100,000
//modulus operator(returns the reminder)
console.log(a%b) //0

```

**STRING OPERATOR**

The string operator ```+``` is used to concatenate, that is, to join string variables together or a string variable to a number e.g

```
//joining 2 strings together
var fname="Felix"
var sname="Ada"
console.log(fname + " " + sname) //output: Felix Ada

//joining a number to a string
console.log("Felix"+99) //output: Felix99)
console.log(("Felix "+99) //output: Felix 99)

```

**SHIFT OPERATORS**

It basically shift the bits by a specified number of times towards the left or right direction as in **left shift** ```<<``` **or right shift** ```>>``` e.g

```
var a=8, b=2;
console.log(a<<b) //output: 32
console.log(a>>b) //output: 2

```
That looks confusing?😂...it's quite easy to get the answer I guess, let me teach you😸

```
/*e.g 8<<2
the rhs, 8, is the only number we are dealing with while the lhs, 2, is just
indicating the amount of times we are shifting the bits.

8 in binary is 1000
So, shifting it twice to the left side is basically adding 2 zeros behind so '1000' can be shifted to the left.

Adding 2 zeros behind '1000' makes it '100000' and that is 32 in decimal.

or do 8x2² = 32

Also, 8>>2
8, which is '1000' in binary will be shifted 2 times to the right '10' which is 2 in binary

or you do 8/2² = 2 

This isn't really necessary to know, but just to have an idea on how it works.*/


```

**COMPARISON OPERATORS**

They include operators used to compare two values.

- To check for inequality, you use ```<```, ```>```, ```<=```, ```>=```
- To check equality, you use either ```==``` or ```===```. The double equals to comparison operator ```==``` allows type coercion while the other, ```===``` doesn't. e.g

```
//to check inequality   
var a=7, b= 4
console.log(a>b) //true
console.log(a<b) //false
console.log(a <= b) //false
console.log(a >= b) //true

//to check equality   
var a=6,b="6"
console.log(a==b) //true
console.log(a===b) //false

```

> I discussed type coercion in the Part 2 of this series, you can look it up [here](https://gracious-grace.hashnode.dev/javascript-made-easy-part-2)



**BITWISE OPERATORS**

The 4 major bitwise operators are: 

- ```&``` (AND): returns 1 if both bits are 1, otherwise 0
- ```|``` (OR): returns 1 if either of the bits is 1, otherwise 0
- ```~``` (NOR): returns the reverse as output, changes 1 to 0 and vice versa.
-  ```^``` (XOR): returns 1 if both bits are different, otherwise 0

```
var a=1,b=0;
console.log(a&b) // 0
console.log(a|b) // 1
console.log(~a) // 0
console.log(~b) // 1
console.log(a^b) // 1

```
**LOGICAL OPERATORS**

Logical operator can be used

- ```||``` (OR): returns true when either of the conditions is true.

- ```&&``` (AND): returns true when both the conditions are true.

- ```!``` (NOT): returns false when condition is true and vice-versa.

**Example:**

```
let occ = "coder"
let age = 20
//OR operator
if (occ == "coder" || age <= 19){
   console.log("You are qualified for the training")
}
else{
   console.log("get away")
}
//output: You are qualified for the training

//AND operator
if (occ == "coder" && age <= 19){
   console.log("You are qualified for the training")
}
else{
   console.log("get away")
}
//output: get away

//NOT operator
let x=9, y=3
console.log(!(x === y)) // true
console.log(!(x > y)) // false

```

**TERNARY OPERATORS**

Ternary operators is another form of using ```if``` ```else```. Condition is usually placed before ```?```, and if it evaluates to true, the LHS of the column ``:``` gets executed, otherwise RHS will be executed. e.g

```
var a=3
console.log((a==3)? console.log("correct"):console.log("not ok"))
//output: correct
```

**TYPE OPERATORS**

- **typeof():** returns the type of a variable. e.g

```
var x=9
document.write(typeof(x)) //output: number
//
var username = "Ada"
document.write(typeof(username)) // output: string


```

- **instanceof**: returns true if an object is an instance of an object type and returns false if otherwise.

```
let lang = ["Python", "Java", "JavaScript"]
    console.log (lang instanceof Array) //true
    console.log (lang instanceof Object) //true
    console.log(lang instanceof String) //false
    console.log(lang instanceof Number) //false

```

I will stop here for today and forge ahead in the part 4 of this series. I really hope you enjoyed reading this article and you learnt new ideas. Feel free to ask questions in the comment section below. Bye👋
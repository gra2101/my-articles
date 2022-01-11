## Javascript Made Easy: Part 2

Hey there! Welcome back. Still walking you through JavaScript, I hope you grabbed some knowledge in the previous [post](https://gracious-grace.hashnode.dev/introduction-to-javascript) of this series, where I briefly discussed:
- What is JS?
- History of JS
- ECMA
- JS development tools and;
- Different places we can type in JS code

Today, we will be digging deeper into JS, so let's get started😀.

## PART 2: 

### JAVASCRIPT COMMENTS
Comments are human readable language in JavaScript which are used to explain or label a line of code in other to make a program more readable for other developers.

Comments are usually not affected during execution, they are usually ignored.

 There are two types of comment:

1. **Single line comment**
2. **Multiple line comment**

**- SINGLE LINE COMMENT**

 Single line comments contain one or a part of one line and are mostly used to label the next code and it is denoted by using ```// ```
e.g

```
// how to print hello on the console
console.log("Hello")

``` 
 
**- MULTIPLE LINE COMMENT** 

Multiple line comments usually contain more than one line. You can comment out a block of code to avoid execution. Multiple line comments can also be used for formal documentation of JS code. It is denoted by ```/* ......*/``` e.g

```
/* This is a multiple line 
   comment. This comment
   is for the purpose of
   demonstration*/

``` 


### JAVASCRIPT OUTPUT

We can display data in JS with the following commands:

1.
 **console.log()**

This command is used to print data on the browser's console page and note that whatever data you want it displayed or printed must be within the braces() of this command. Watch:


```
//how to use console.log()
console.log("Hello JavaScript")
``` 


> 
To locate the console, open the HTML file of which you have linked your JS code on your browser and press 
```ctrl```+```shift```+```i``` 



2.
 **document.write()**

The document.write() command is used to display data on the page of a browser. Whatever data you want it displayed or printed must be within the braces() of this command.

```
//how to use document.write()
document.write("Hello JavaScript")

``` 

3.
 **window.alert()**

This command is used to display data on an alert box that pops up on the browser's page.


```
//how to use window.alert()
window.alert("Hello World")
```
and the output is usually like this👇

![alertDemo.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1621514705280/CmE1jVK6Y.png)


 
4.
**.innerHTML**

JavaScript uses the ```document.getElementById("id")``` method to access an HTML element and displays data in the HTML tag in which the ID is allocated to. e.g
<iframe height="265" style="width: 100%;" scrolling="no" title="innerHTML" src="https://codepen.io/gra2101/embed/VwpPjLJ?height=265&theme-id=dark&default-tab=js,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/gra2101/pen/VwpPjLJ'>innerHTML</a> by Grace O.
  (<a href='https://codepen.io/gra2101'>@gra2101</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>


### JAVASCRIPT PROPERTIES

1.
**JavaScript is dynamically typed**, meaning, you do not have to specify the type of variable you are declaring because JS automatically detects that itself during runtime e.g
```var myName = "Grace"
```  In this case, JavaScript automatically detects ```"Grace"``` as a string value without a need to state it. Unlike Java, where you have to declare the type of data before declaring it like ```String myName="Grace"```(this makes java a **Static typed** programming language)

2.
**JavaScript is weakly typed**, meaning datatype coercion in JS is allowed. **What is Coercion?** Coercion is the conversion of a value of one datatype to the same value of another datatype.

In JS, triple equals sign ```===```
is used to stop datatype coercion.

<iframe height="265" style="width: 100%;" scrolling="no" title="JS type_coercion" src="https://codepen.io/gra2101/embed/abJpVqM?height=265&theme-id=dark&default-tab=js,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/gra2101/pen/abJpVqM'>JS type_coercion</a> by Grace O.
  (<a href='https://codepen.io/gra2101'>@gra2101</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### JAVASCRIPT DATA TYPES

There are two types of data in JS; **primitive** and **non-primitive** datatypes. 

1.
**PRIMITIVE DATA TYPE**

A Primitive data type is a fundamental data type that cannot be broken down into a more simple data type. 
In JS, data types that fall here are:

- **STRING** mostly made up of text characters. String can also contain numbers; any character in quotes is automatically a string datatype. e.g ```"Alex"```, ```"Grace22"```,  ```"95"```
- **NUMBER** can be an integer(a number with no decimal point) or float(a number with decimal point) e.g ```721```, ```15.79```
- ** BOOLEAN** values can be either ```true``` or ```false```
- **BIGINT** is a special numeric type that provides support for integers of arbitrary length. This data type allows us to safely perform arithmetic operations on large integers like mathematical operations used in financial technology, for example.
- **UNDEFINED** is given when a variable is declared but has no value attached to it yet. e.g ```var message;```, then message has an undefined datatype.
- **NULL**, you can assign the value **null** to any variable which basically means it's blank, you have intentionally made it empty. e.g ```var age=null```
- **SYMBOLS** are used to create a unique properties of objects. e.g

<iframe height="265" style="width: 100%;" scrolling="no" title="JS Symbol" src="https://codepen.io/gra2101/embed/VwpPEEV?height=265&theme-id=dark&default-tab=html,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/gra2101/pen/VwpPEEV'>JS Symbol</a> by Grace O.
  (<a href='https://codepen.io/gra2101'>@gra2101</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

The example above without ```Symbol``` is meant to output ```true```, but the ```Symbol``` we included created a distinctive property and made these two values uniquely defined, thus, giving a false output.

2.
**NON-PRIMITIVE DATA TYPE**

Non-primitive types can be used to call methods to perform certain operations. They are usually created by the programmer.

- **OBJECT** in JavaScript is a collection of properties, where each property is defined as a key-value pair. An object is usually represented with curly braces ```{}```e.g

```
let person = {
     name: "grace"
     age: 19
     married: false
}

```
> ```let``` is also a keyword that can be used instead of ```var``` but have different functions, I will discuss that later in this series.

- **ARRAY**
An array is a data type that can contain multiple data types. An array is usually represented with a square bracket ```[]``` with each of the items in the array separated by a comma e.g


```
//array of numbers
let myFavNumbers=[2,4,6,8,10]

//array of strings
let myFavNames=['Grace', 'Carissa', 'Alex']

//array of mixed datatype
let array1=['name', 20, 'food']

``` 


### JAVASCRIPT VARIABLES

A Variable can be defined as the memory location of a computer. We can see a variable as a container for storing data. A variable in JS is defined as ```var``` e.g

```var myName = "grace"```

```var age = 19```

- ```"grace"``` will be stored in the variable named ```myName```
- ```19``` will be stored in the variable named ```age```
 
### JAVASCRIPT NAMING CONVENTION
Observe the following rules when naming a variable in JavaScript:

1.
Names must begin with a letter or a dollar sign ```$``` or an underscore ```_```

2.
Names are case sensitive (x and X are different variables)

3.
A variable name must not be the same as a keyword. e.g using ```var``` as a variable name.

4.
Use camel casing in JavaScript when your variable name contains two words or more e.g ```camelCasing```



> Keywords in JavaScript are words built with JS. They are reserved words used to perform specific functions. Keywords are part of the syntax and they cannot be used as an identifier(name of a variable, function, array and so on).

I hope you learnt something new. See you in my [next](https://gracious-grace.hashnode.dev/javascript-made-easy-part-3) post.😊







# Week 1

## JavaScript Basic Overview

- JavaScript was initially created to add “dynamics” to a web page
- The programs in this language are called scripts
- They can be written right in the HTML and execute automatically as the page loads
- Scripts are provided and executed as a plain text
- They don’t need a special preparation or a compilation to run
- In this aspect, JavaScript is very different from another language called Java
- Client-Side which means the code is interpreted by the browser

### Code Editors

Everyone has a preference for code editors, you are free to work in any of these but Visual Code Studio will be what we use in all of the tutorial videos.

- Visual Studio Code
- Notepad++
- Brackets
- Sublime

### Developer Console

The console is a tool that developers use to record the output of their JS programs. The link below is helpful in reference to developer tools, please make sure to activate the developer tools when working with JavaScript code.

- https://javascript.info/devtools

### Data types

Data Types are the building blocks of all languages and essential pieces of any program
There are 4 primitive data types:

1. String
2. Number
3. Boolean
4. Null

### Syntax

JavaScript can be implemented using JavaScript statements that are placed within the <script>…</script> HTML tags in a web page. You can place the <script> tags, containing your JavaScript anywhere within your web page, you will learn throughout this course the best placement of the script which depends upon the goal of the page.

The <script> tag alerts the browser program to start interpreting all the text between these tags as a script. A simple syntax of your JavaScript will appear as follows:

```
<script ...>
	//Javascript Code
</script>
```

There are two attributes that are included within a web page:

1. Language
   - This attribute specifies what scripting language you are using, which typically, its value will be JavaScript
2. Type
   - Indicates the scripting language being used on the web page

The code below is an example of the script tags within the web page:

```
<script language="javascript" type="text/javascript">
	//Javascript Code
</script>
```

### White Space and Line Breaks

JavaScript ignores spaces, tabs, and newlines that appear in JavaScript programs. You can use spaces, tabs, and new lines freely in your program and you are free to format and indent your programs in a neat and consistent way that makes the code easy to read and understand.

### Case Sensitivity

JavaScript is a case-sensitive language. This means that the language keywords, variables, function names, and any other identifiers must always be typed with a consistent capitalization of letters. So the identifiers Time and TIME will convey different meanings in JavaScript.

### Comments

Programs do not evaluate comments, they are useful for you and other programmers.
Examples:

```
// Single Line Comment

/*
 This is for a multiline comment
 Nothing inbtween the starting and ending /* will be run by the program
*/
```

### Enabling

All of the modern browsers come with built-in support for JavaScript. Frequently, you may need to enable or disable this support manually.

#### Firefox

Open a new tab -> type about: config in the address bar. Then you will find the warning dialog. Click the button and view the list of configure options in the browser. In the search bar, type javascript.enabled. There you will find the option to enable or disable JavaScript by right-clicking on the value of that option -> select Toggle.

![](Screenshot%202023-08-27%20at%202.05.45%E2%80%AFPM.png)
![](Screenshot%202023-08-27%20at%202.09.51%E2%80%AFPM.png)

#### Chrome

Chrome menu > Settings > Show advanced settings > Privacy > Content Settings Button > JavaScript section select:

- Do not allow any site to run JavaScript
- Allow all sites to run JavaScript (recommended)

## Activity

Let’s start by typing some basic JavaScript code that will print to the web console area.
Use the code below as a guide to create your first JavaScript code.

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>JavaScript Language Basics</title>
    </head>

    <body>
        <h1>JavaScript Language Basics</h1>
		 <!-- adding inline Javascript code must be enclosed in script tags -->
		<script>

		</script>
    </body>

</html>

```

Save the file as JavaScript_WeekOne_CodePractice.html ~ I will not include save and refresh with my instructions, you should be proficient with these steps already

Launch the code using your browser of choice, ( My screen shots will always be Chrome )

Modify the code using the code as a guide:

```
<!-- adding inline Javascript code must be enclosed in script tags  -->
<script>
	console.log('Hello world!'); // standard text
</script>
```

**Results ~**
![](Screenshot%202023-08-27%20at%202.19.34%E2%80%AFPM.png)

Modify the code using below as a guide:

```
<script>
	console.log("Hello World"); // standard text
	console.log(3.5+23); // add 3.5 to your age
	console.log(2023-1969); // subtract 1969 from the current year
	console.log(2.708*100); // multiply 100 by 2.708
</script>
```

**Results ~**
![](Screenshot%202023-08-27%20at%202.23.03%E2%80%AFPM.png)

The console is a great tool, notice how it provides you with the result of your code along with the filename and line number. This will become quite handy when your code contains errors.

Another web site that should be in your bookmarks is ~ https://developer.mozilla.org/enUS/docs/Web/JavaScript/Reference/Global_Objects/String/prototype

With these next exercises, you will explore the web site and implement properties and methods. Continue to code on your own.

**Properties**
Every string instance has a property called length, which stores the number of characters of the string.

`console.log(‘JavaScript is Fun to Learn!’.length);`

**Methods**
Methods are like verbs, they perform actions that generate output.

`console.log(‘hello’.toUpperCase()); //HELLO`
In this example, the .toUpperCase method is called on the string ‘hello’ and returns to the console the letters in uppercase

Which method would I use to fix the following?

- `console.log(' Remove whitespace '.trim());`

**Libraries**
Contain methods that you can call without creating an instance

Use the Math Library to explore the methods ~ [Math - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)

`console.log(Math.random()); // random number between 0 and 1`

What if you wanted to generate a random number between 0 and 50?

- `Math.random() * 50; //the answer will be a decimal`

To ensure whole numbers, another built-in method can be used Math.floor(), which rounds-down to the nearest whole number.

- `Math.floor(Math.random() * 50);`

Create a random number with the Math.random() method and multiply it by 100

- `console.log(Math.random() *100);`

Use the Math.floor method to make the output a whole number

- `console.log(Math.floor(Math.random() *100))`

Find a method in the JS Math Library that returns the smallest integer greater than or equal to a decimal number; Use this method with the number 43.8.

- The Math.ceil() function returns the smallest integer greater than or equal to a given number

Find a method in the Number library that checks if a number is an integer

- `console.log(Number.isInteger(34.2));`
- Use the number 2017

If you make errors in your code, the console presents you with an error alert, which provides a hint to the error along with the line number ~
![](Screenshot%202023-08-27%20at%202.31.33%E2%80%AFPM.png)

## Summary

- Four essential data types in JavaScript include strings, numbers, booleans, and null.
- Data is printed, or logged, to the console with console.log().
- Four built-in mathematical operators include +, -, \*, and /.
- JavaScript associates certain properties with different data types.
- JavaScript has built-in methods for different data types.
- Libraries are collections of methods that can be called without an instance.
- You can write single-line comments with // and multi-line comments between /_ and _/.

These activities must be submitted through Github classroom and marked as done in the assignment in Blackboard.

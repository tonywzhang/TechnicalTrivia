# Technical Trivia

* Why do you need a doctype?

 * Doctype is an instruction to the browser to inform about the version of the html document and how the browser should render it.

* What is the use of the data-* attribute?
  * It allows you to store extra information/data in the DOM. You can write valid html with embedded private data. You can easily access the data attribute by using javascript and hence a lot of libraries like knockout use it.

* What is createDocumentFragment?
  * createDocumentFragment is like a mini DOM you can append elements to in order to avoid costly insertions. Once you've appended elements to the fragment, you can append the fragment to a node element and the fragment itself with disappear.

* What does float do?
  * Float removes the element from the normal flow of the document and pushes the element to the sides of the page with text wrapping around it.

* Are CSS properties case sensitive?
  * No.

* What is position static?
  * The default position value for an html element. Not relative, absolute, fixed, or sticky.

* Is there implicit function return in JavaScript?
  * Yes, via one line big arrow functions or big arrow functions that wrap their block in parentheses.

* How can you apply css rules specific to media/screen-size?
  * Use @media to set rules based on media width, orientation, etc.
  * Example: @media (max-width: 700px) and (orientation: landscape){}

* What are the 7 falsey values in JavaScript?
  * 0, "", NaN, -0, null, undefined, false

* What is a primitive datatype in JavaScript?
  * A primitive datatype is not an object, is immutable, and has no attributes/methods directly defined on it.

* Consider the following expression: var y=1, x=y=typeof x. What will be the value of x?
  * undefined

* If const a = 2, b = 3, what would be the value of a && b ?
  * 3

* Is null an object?
  * No. Even though typeof null returns object, this is a bug. You cannot put any attributes on null, as it is a primitive datatype.

* Are let and const hoisted?
  * Yes.

* Describe memoization
  * Memoization is a programming technique which attempts to increase a function's performance by caching its previously computer results. POJO's are often used to implement these caches.

* How can you change the direction of html text?
  * use bdo (bidirectional override) element of html.
  * <p><bdo dir="rtl">This text will go right to left.</bdo></p>

* How can you highlight text in html?
  * Use mark element.
  * <p> Some part of this paragraph is <mark> highlighted <mark/> by using mark elemnet. <p/>

* Does margin-top or margin-bottom affect inline elements?
  * No.

* What is position relative?
  * The computed position of the element where it can be spaced in relation to its' normal position in the flow of the document using top, bottom, left, and right.

* Name three pseudo-selectors:
  * :hover, :visited, :focus, :link, :first, :checked, etc.

* Name all six primitive data-types in JavaScript:
  * boolean, string, number, null, undefined, and symbol

* What is the difference between  null and undefined ?
  * Undefined means the value of the variable is not defined. JS has a global variable called undefined whose value is undefined.
  * null means empty or non-existent value which is used by programmers to indicate "no value".

* What is the value of this inside of a setTimeout function?
  * The window itself.

* What is the value of this inside of a constructor function?
  * A newly created object

* What is the temporal dead zone?
  * This has to do with the topic of hoisting. The temporal deadzone is the time between entering a scope where a variable is declared (i.e. an if statement or while loop), and the actual declaration and initialization of that variable. During this period, let and const variables cannot be accessed (you will get a Reference Error), even though they have been hoisted.

* What is position absolute?
  * The computed position of the element where it can be spaced after being removed to from the normal flow of the document. It is spaced in relation to its' first non-static parent container with top, bottom, left, and right.

* Explain variable hoisting:
  * At a broad level, hoisting is the concept of having access to named functions and variables (only vars) before they are declared in your code. This works because variable and function declarations are put into memory during the compile phase.

* Does javascript pass parameter by value or by reference?
  * It depends on the datatype. Primitive types (string, number, etc.) are passed by value and objects are passed by reference. If you change a property of the passed object, the object will be affected.

* Is Javascript compiled or interpreted?
  * Interpreted.

* What are the three phases of event propagation?
  * Capturing phase: Events begin at the top level and move inwards towards the target (the node you clicked)
  * Target node: If there are registered handlers at the target node, they are run.
  * Bubbling phase: Event walks back outwards towards root; all encountered event handlers are run on the way.

* What does the global object refer to in JavaScript?
  * A POJO that exists to provide all built-in methods and global variables.

* What does the "length" property of the JavaScript Function object return?
  * The number of arguments taken by the function (not including rest parameters)

* What is a prototype in JavaScript?
  * An object.

* What are the differences between div and span?
  * Div is a block element and span is inline element.

* What is the difference between a canvas element and an SVG?
  * SVG: Object Model-based (SVG elements are similar to HTML elements). Graphical elements become part of the DOM. Visual presentation created with markup and modified by CSS or script. API supports accessibility. API does not support accessibility; markup-based techniques must be used in addition to canvas.

  * Canvas: Pixel-based (canvas is essentially an image element with a drawing API). Single HTML element similar to  in behavior. Visual presentation created and modified programmatically through script.

* Do padding-left, padding-right, margin-left, or margin-right effect inline elements?
  * Yes.

* Why can we call methods on certain primitive datatypes?
  * Technically, you can't.
  * Certain primitive datatypes, like strings, numbers, and booleans, have non-primitive counterparts (String, Number, Boolean). So, if you call "string".slice(5), that string will be implicitly cast to a String object, and the slice method will be called on that.

* What is position fixed?
  * The computed position of an element where it's position is constant or 'fixed' in relation to the window. Its' position and presence never change.

* What is position sticky?
  * It's treated as relatively positioned until its containing block crosses a specified threshold (such as setting top to value other than auto) within its flow root (or the container it scrolls within), at which point it is treated as "stuck" (it doesn't move) until meeting the opposite edge of its containing block.

* What are the differences between == and === ?
  * == will not check types and === will check whether both sides are of same type. == will convert to its convenient type to have both in same type and then do the comparison.

* If you create a function that takes 2 arguments, but invoke it with 3 arguments, how can you access the third variable?
  * Use the "arguments" keyword.

* What is NaN? What is its type? How can you reliably test if a value is equal to NaN?
  * NaNs type is Number. NaN compared to anything, even itself, is false. One way to check if they are equal is using the built in isNaN() function.

* What is a closure in javascript?
  * A closure is an inner function that has access to the variables in the outer (enclosing) function’s scope chain. The closure has access to variables in three scopes; specifically: (1) variable in its own scope, (2) variables in the enclosing function’s scope, and (3) global variables.

* When you zoom in on your browser and the page gets bigger, what exactly happens?
  * The browser increases the size of each pixel by the percentage of the zoom.

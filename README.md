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

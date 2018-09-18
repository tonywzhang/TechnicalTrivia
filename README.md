# Technical Trivia

* Why do you need a doctype?

 * Doctype is an instruction to the browser to inform about the version of the html document and how the browser should render it.

* What is the use of the data-* attribute?
  * It allows you to store extra information/data in the DOM. You can write valid html with embedded private data. You can easily access the data attribute by using javascript and hence a lot of libraries like knockout use it.

* What is createDocumentFragment?
  * createDocumentFragment is like a mini DOM you can append elements to in order to avoid costly insertions. Once you've appended elements to the fragment, you can append the fragment to a node element and the fragment itself with disappear.

* What does float do?
  * Float removes the element from the normal flow of the document and pushes the element to the sides of the page with text wrapping around it.

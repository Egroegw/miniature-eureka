# README
This is the README for CS279r, Fall 2022, with Elena Glassman and TF Priyan Vaithilingam.

## Usage instructions
To open the TODO app, open `279.0.html` in a web browser.

The app contains two lists, **current** tasks and **finished (archived)** tasks, plus a rubbish bin if you accidentally delete a task.

* You can always add a task to the list of _current_ tasks by write it in the text box and clicking "Add task"

### Current tasks
* To mark a task complete, click the "Mark complete" button next to that task
* To delete a task from the task list, click the "Delete" button next to that task

### Completed (archived) tasks
* To mark a task incomplete, click the "Mark incomplete" button next to that task
* To delete a task from the task list, click the "Delete" button next to that task

### Deleted Tasks
* To restore a deleted task to the list of current tasks, click "Restore to task list"
* To delete a task permanently, click "Delete permanently"


Tasks that are marked complete are moved to the Archive. Tasks that are deleted are moved to the Rubbish Bin.

## Explanatory Notes and Sources

As I have never written more than "Hello World!" in Javascript before, this first problem set was an interesting challenge. The language I come from is Python, but I am also learning Rust.

I did not follow any tutorials in writing this application. I relied on https://developer.mozilla.org/en-US/docs/Learn as well as https://www.w3schools.com/html/ and https://www.w3schools.com/js/.

My initial plan was to
1. understand how to store text and items in Javascript
2. understand how to incorporate Javascript into an HTML document, and
3. understand how to use CSS to improve the visual and aesthetic nature of the TODO list.

The reason I put CSS last was that I assumed functionality came before aesthetics.

The initial tutorial/introduction to Javascript I used was w3schools.com's. Unfortunately, w3schools.com's tutorial is incomplete, poorly written, and omits basic syntax such as `for (var item of array)`. Consequently, halfway through, I ran to Mozilla's tutorial instead: https://developer.mozilla.org/en-US/docs/Web/JavaScript/.

### Incorporating Javascript into an HTML document
Well, this turned out to be simpler than expected. Simply place content inside enclosing `<script>` tags: `<script> // some Javascript function or variable </script>`.

JS can be inline, or in an external file.

https://www.w3schools.com/html/html_scripts.asp

### Storing text and items in Javascript
This was somewhat more difficult than embedding Javascript. Surprisingly, Javascript doesn't have Python lists: it has arrays instead.

https://www.w3docs.com/snippets/javascript/how-to-get-the-value-of-text-input-field-using-javascript.html

.findIndex() and .splice() were extremely useful methods that allowed me to move items from one array to another.

### CSS
CSS was relatively easier to work with. The main visual change I made was to force all text to be sans-serif. Supposedly sans-serif text works better on screens with less resolution, but it's also an excuse for me to play around with the font-family. 

Not strictly related to this assignment, but I also consulted Matthew Butterick's ebook at https://practicaltypography.com.

### Misc. notes

* I kept using .Trim() on a string instead of .trim()
* In Rust, the final expression is automatically returned， without needing the "return" keyword. I forgot to use the "return" keyword in isEmptyString() for a long time. 
* There are four ways to "print" something in Javascript, none as simple as Python's print().
* In Javascript, the top-to-bottom order of your functions matters. You cannot invoke a function before it has been defined, unlike in Rust.
* Be extremely aware of strings and escaped characters.
* Try your utmost to break lines at opportune locations.
* You debug more if you subbornly try to write in a new language as if you were writing in a familiar language.

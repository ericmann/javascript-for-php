##  Prototypes

<pre><code lang="js">function Book( title, author ) {
    this.title = title;
    this.author = author;    
    this.page = 0;
    
    this.read = function() {
        this.page += 1;
    };
}

var myBook = new Book( 'How to Write JavaScript', 'Eric Mann' );

console.log( myBook );
// Book {title: "How to Write JavaScript", author: "Eric Mann", page: 0}

myBook.read();

console.log( myBook.page );
// 1

Book.prototype.restart = function() {
    this.page = 0;
};

myBook.restart();

console.log( myBook.page );
// 0</code></pre>

note:
    JavaScript handles inheritance a bit differently than other languages - it uses a _prototype chain_ to define how things are inherited. When a property or method is invoked, the interpreter first looks at the object itself. If the definition isn't there, JS then checks the object's prototype, then the prototype's prototype, and so on, until either the definition is found or the next prototype in the chain is null. 
    
    In the above example, the `Book` implementation has only one method, `::read()`, but its _prototype_ (`Object` by default) has a `::restart()` method as well.
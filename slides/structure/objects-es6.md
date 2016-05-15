##  Objects

<pre><code lang="js">class Book{
    constructor( title, author ) {
        this.title = title;
        this.author = author;    
        this.page = 0;
    }
    
    read() {
        this.page += 1;
    }
}

// `let` is a scoped alternative to `var`
let myBook = new Book( 'How to Write JavaScript', 'Eric Mann' );

console.log( myBook );
// Book {title: "How to Write JavaScript", author: "Eric Mann", page: 0}

myBook.read();

console.log( myBook.page );
// 1

myBook.restart = function() {
    this.page = 0;
};

myBook.restart();

console.log( myBook.page );
// 0</code></pre>

note:
    In ES6, you can define an object class as just that, a class. This brings us even closer in alignment with the way PHP does things. Only keep in mind that you need a `constructor` method instead of `__construct` and that there is no sense of "private" or "protected" in this kind of definition.

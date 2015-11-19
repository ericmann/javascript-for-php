##  Objects

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

myBook.restart = function() {
    this.page = 0;
};

myBook.restart();

console.log( myBook.page );
// 0</code></pre>

note:
    Objects can be defined by building a constructor function and prepending that function's invocation with the `new` keyword. These objects work exactly the same as any other.

##  Objects

<pre><code lang="js">// book.js
let books = 0;

class Book{
    constructor( title, author ) {
        this.title = title;
        this.author = author;
        this.page = 0;
        books += 1;
    }
    
    read() {
        this.page += 1;
    }
    
    static counter() {
        return books;
    }
}

// main.js
import Book from './book';

// `let` is a scoped alternative to `var`
let myBook = new Book( 'How to Write JavaScript', 'Eric Mann' );

console.log( myBook );
// Book {title: "How to Write JavaScript", author: "Eric Mann", page: 0}

myBook.read();

console.log( myBook.page ); // 1

console.log( Book.counter() ); // 1</code></pre>

note:
    In ES6, you can define an object class as just that, a class. This brings us even closer in alignment with the way PHP does things. Only keep in mind that you need a `constructor` method instead of `__construct` and that there is no sense of "private" or "protected" in this kind of definition.

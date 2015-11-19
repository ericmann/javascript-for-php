##  Objects

<pre><code lang="js">var myArray = {
    'classification': 'fruit',
    'type': 'orange',
    'eat': function() {
        // ...
    }
};

console.log( myArray );
// Object {classification: "fruit", type: "orange"}

myArray.eat();
// Does whatever ::eat() does.

myArray.restock = function() {
    // ...
};

myArray.restock();
// Does whatever ::restock() does.</code></pre>

note:
    Objects can either be defined in pieces as with the previous example or as literals using JSON format. Functions are first-class members of JS and can be assigned to variables, object properties, or declared directly as expressions. Objects can also have their members dynamically redefined later.

##  Arrays

<pre><code lang="js">var myArray = [];
myArray[0] = 'orange';
myArray[1] = 'apple';
myArray.push( 'banana' );

console.log( myArray );
// ['orange', 'apple', 'banana']

myArray[1] = 'grape';

console.log( myArray );
// ['orange', 'grape', 'banana']

console.log( myArray.length );
// 3</code></pre>

note:
    The thing to note here is how `myArray` is itself an object with its own methods. Instead of calling external functions to `::push()` or calculate `::length` you can access these components directly.

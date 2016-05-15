##  References

Variables are passed by _reference_ ...

<pre><code lang="php">var firstArray = ['Element'];
var secondArray = firstArray;

secondArray.push( 'Another' );

console.log( firstArray );
// ['Element', 'Another']</code></pre>

note:
    In PHP, you often have to specify whether variables are being used by value or by reference. In JavaScript, references are the default.

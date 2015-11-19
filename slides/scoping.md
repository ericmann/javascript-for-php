##  Scoping

<pre><code lang="js">function definer() {
    myVal = 5;
    window.otherVal = 10;
    
    var privateVal = 20;
}

console.log( myVal );      // ERROR
console.log( otherVal );   // ERROR
console.log( privateVal ); // ERROR

definer();

console.log( myVal );      // 5
console.log( otherVal );   // 10
console.log( privateVal ); // ERROR</code></pre>

note:
    Variables defined inside a function (or object constructor) are private only to that context. Anything without the `var` keyword, though, can accidentally be added to the global scope!

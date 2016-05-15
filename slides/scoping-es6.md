##  Scoping

<pre><code lang="js">let myVal = 5;
let iterable = [1,2,3,4,5];

for ( let val of iterable ) {
    var exposed = val * myVal;
    let hidden = val * myVal;
        
    console.log( [ exposed, hidden ] );
}
    
console.log( exposed ); // 25
console.log( hidden );  // ERROR

// `let` is used once and only once per scope
var first = 5;
let second = 10;

var first = 15;  // OK, but dumb
let second = 20; // ERROR

do {
    let second = 20;       // OK
    
    console.log( second ); // 20
} while ( false );

console.log( second ); // 10</code></pre>

note:
    The `let` keyword is safer to use than `var` as its scope is set. That's to say it won't ever bleed outside of the scope in which you're using a variable. But unlike `var`, you'll receive a Type Error if you try to redeclare an already-scoped variable.

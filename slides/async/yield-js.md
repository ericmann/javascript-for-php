## Yield

The `yield` keyword and the `function*` construct power the creation of generators.

<pre><code lang="js">function* gen() {
    yield 1;
    yield 2;
                      
    yield 3; // The last item in JS should still be yield
}
                      
for (let val of gen() ) {
    console.log( val );
}</code></pre>
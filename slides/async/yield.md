## Yield

The `yield` keyword powers the creation of generators

<pre><code lang="php">$gen = (function() {
    yield 1;
    yield 2;
                      
    return 3;
})();
                      
foreach ($gen as $val) {
    echo $val, PHP_EOL;
}
                      
echo $gen->getReturn(), PHP_EOL;</code></pre>
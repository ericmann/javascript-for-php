##  Arrays

<pre><code lang="php">$myArray = array();
$myArray[0] = 'orange';
$myArray[1] = 'apple';
array_push( $myArray, 'banana' );

print_r( $myArray );
// Array( [0] => 'orange' [1] => 'apple' [2] => 'banana' )

$myArray[1] = 'grape';

print_r( $myArray );
// Array( [0] => 'orange' [1] => 'grape' [2] => 'banana' )

echo count( $myArray );
// 3</code></pre>

note:
    PHP supports indexed arrays very nicely, and this example can be illustrated almost 11:1 in JavaScript.

##  Objects

<pre><code lang="js">var myArray = {};
myArray['classification'] = 'fruit';
myArray['type'] = 'orange';

console.log( myArray );
// Object {classification: "fruit", type: "orange"}

console.log( myArray.classification );
// "fruit"
</code></pre>

note:
    Unfortunately, JavaScript doesn't support _associative_ arrays. Instead, you can use an Object as kind of a hash table to get the same support. Conveniently, once you're using an object, you can reference properties on it just like any other.

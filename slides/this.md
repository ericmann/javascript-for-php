##  This

<ul>
    <li class="fragment">In PHP, `$this` is a reference to the current object</li>
    <li class="fragment">In JavaScript, `this` is a _context_ reference</li>
    <li class="fragment">TL;DR; Be explicit as often as possible!</li>
</ul>

note:
    In click events, `this` is a reference to the element that was clicked. In an object constructor, it's a reference to the object being constructed. In a function invocation it's a reference to the caller. `this` is ... not always what you think it is.

0.  What's the difference between `call()` and `apply()`?
    How and why would you use them?

0.  Write a function that tells me if a word is an anagram or a palindrome of another word.

    A palindrome is a word that you can read both ways (e.g. `abba`).
    An anagram is a word that contains every letters of another word (e.g. `rome` and `more`).

    Example:

    ```javascript
    is_anagram_or_palindrome(word_a, word_b); // true or false
    ```

    NB: You don't need to do parameters validation.

0.  One of these assertions will fail. Which one and why?

    ```javascript
    // Returns true if thing is an object
    function is_object(thing) {
        return thing && Object.prototype.toString.call(thing) === '[object Object]';
    }

    console.assert(is_object([]) === false               , 'assert #1');
    console.assert(is_object({}) === true                , 'assert #2');
    console.assert(is_object(null) === false             , 'assert #3');
    console.assert(is_object(new function () {}) === true, 'assert #4');
    ```

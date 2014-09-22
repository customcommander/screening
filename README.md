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

0.  This is the content of a file named **foo.js**:

    ```javascript
    function foo() {
        (function () {
            alert('hello world');
        })();
    }
    ```

    And this is **foo.html**:

    ```html
    <!DOCTYPE html>
    <html>
        <head>
            <script src="foo.js"></script>
        </head>
        <body></body>
    </html>
    ```

    What happens when **foo.html** is loaded in a web browser?

0.  What is the output of the following program?

    ```javascript
    function foo() {
      return new bar();
    }

    function bar() {
      return {};
    }

    function baz() {
    }

    var a = new foo();
    var b = new bar();
    var c = new baz();

    try {
      console.log('#1: ', a instanceof foo ? 'yes' : 'no');
      console.log('#2: ', a instanceof bar ? 'yes' : 'no');
      console.log('#3: ', b instanceof bar ? 'yes' : 'no');
      console.log('#4: ', c instanceof baz ? 'yes' : 'no');
    } catch (e) {
      console.log('err!');
    }
    ```

0.  Which of the following assertions will fail?

    ```javascript
    function assert_equal(a, b, message) {
        if (a !== b) {
            console.log(message);
        }
    }

    assert_equal(true    , true     , 'test #1');
    assert_equal(true    , 1        , 'test #2');
    assert_equal([1,2]   , [1,2]    , 'test #3');
    assert_equal({}      , {}       , 'test #4');
    assert_equal(10      , '10'     , 'test #5');
    assert_equal('foo'   , 'foo'    , 'test #6');
    assert_equal(Infinity, Infinity , 'test #7');
    assert_equal(null    , undefined, 'test #8');
    assert_equal(NaN     , NaN      , 'test #9');
    assert_equal(1.0     , 1        , 'test #10');
    ```


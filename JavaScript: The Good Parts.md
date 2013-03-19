**JavaScript: The Good Parts**, by *Douglas Crockford*

A common error in JavaScript programs is to use an object when an array is required or an array when an object is required. The rule is simple: when the property names are small sequential integers, you should use an array. Otherwise, use an object.

---

Regular expressions came from the mathematical study of formal languages. Ken Thompson adapted Stephen Kleene's theoretical work on type-3 languages into a practical pattern matcher that could be embedded in tools such as text editors and programming languages.

---

Sloppy regular expressions are a popular source of security exploits.

---

Regular expressions are best when they are short and simple. Only then can we have confidence that they are working correctly and that they could be successfully modified if necessary.

---

There is a very high degree of compatibility between JavaScript language processors. The part of the language that is least portable is the implementation of regular expressions. Regular expressions that are very complicated or convoluted are more likely to have portability problems. Nested regular expressions can also suffer horrible performance problems in some implementations. Simplicity is the best strategy.

---

JavaScript is a prototypal language, which means that objects inherit directly from other objects.

---

If we create an object in the functional style, and if all of the methods of the object make no use of this or that, then the object is durable. A durable object is simply a collection of functions that act as capabilities. A durable object cannot be compromised. Access to a durable object does not give an attacker the ability to access the internal state of the object except as permitted by the methods.

---

This is differential inheritance. By customizing a new object, we specify the differences from the object on which it is based.

---

The lineage of an object is irrelevant. What matters about an object is what it can do, not what it is descended from.

---

there is a convention that all constructor functions are named with an initial capital, and that nothing else is spelled with an initial capital. This gives us a prayer that visual inspection can find a missing new. A much better alternative is to not use new at all.

---

The general pattern of a module is a function that defines private variables and functions; creates privileged functions which, through closure, will have access to the private variables and functions; and that returns the privileged functions or stores them in an accessible place.

---

Number.method('integer', function (  ) {     return Math[this < 0 ? 'ceil' : 'floor'](this); });

---

There are four patterns of invocation in JavaScript: the method invocation pattern, the function invocation pattern, the constructor invocation pattern, and the apply invocation pattern. The patterns differ in how the bonus parameter this is initialized.


[JavaScript: The Good Parts](https://readmill.com/books/javascript-the-good-parts)
**JavaScript: The Good Parts**, by *Douglas Crockford*

The lineage of an object is irrelevant. What matters about an object is what it can do, not what it is descended from.

---

there is a convention that all constructor functions are named with an initial capital, and that nothing else is spelled with an initial capital. This gives us a prayer that visual inspection can find a missing new. A much better alternative is to not use new at all.

---

This is differential inheritance. By customizing a new object, we specify the differences from the object on which it is based.

---

Number.method('integer', function (  ) {     return Math[this < 0 ? 'ceil' : 'floor'](this); });

---

JavaScript is a prototypal language, which means that objects inherit directly from other objects.

---

If we create an object in the functional style, and if all of the methods of the object make no use of this or that, then the object is durable. A durable object is simply a collection of functions that act as capabilities. A durable object cannot be compromised. Access to a durable object does not give an attacker the ability to access the internal state of the object except as permitted by the methods.

---

There are four patterns of invocation in JavaScript: the method invocation pattern, the function invocation pattern, the constructor invocation pattern, and the apply invocation pattern. The patterns differ in how the bonus parameter this is initialized.

---

The general pattern of a module is a function that defines private variables and functions; creates privileged functions which, through closure, will have access to the private variables and functions; and that returns the privileged functions or stores them in an accessible place.

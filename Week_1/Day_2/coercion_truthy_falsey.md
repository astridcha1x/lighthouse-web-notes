# Equals & Type Coercion
`===` and `==` are two comparative operators to compare values in JavaScript.
- `===` compares the type first, before comparing the actual values itself
  - if they aren't the same type, it will immediately result in false

> `23 === "23"` will result in `false` because `23` is a Number, and `"23"` is a String.

- `==` will first try to force the two values to be of the same type (if possible)
  - this process is **type coercion**, which can produce unexpected results in your code

> `23 == "23"` will result in `true` because `23` (Number) and `"23"` (String) will be coerced to become the same data type.

- Using `===` would be best practice in order to avoid any accidental type coercion in your code


## Not Equal
---
`!==` and `!=` work similarly to the equal comparative operators, including the forced type coercion.
Unless the situation requires type coercion, it is also best practice to use `!==` to avoid any accidental type coercion in your code.



# Truthy & Falsey
Comparing values in JavaScript will return either `true` or `false`. Everything in this language has an inherent Boolean value, which is commonly referred to as a **Truthy** or **Falsey** value.

## The 6 Falsey Value Types
_the following are all inherently falsey._
* `false`
* `0`
* `""` *(empty string)*
* `null`
* `undefined`
* `NaN`
> with these Falsey values in mind, it means that it's safe to assume that a value can be considered **Truthy** if it's not one of the 6 types listed above!
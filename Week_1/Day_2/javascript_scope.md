# Global & Local Scopes
In JavaScript, the two basic levels of scope are **global** and **local**.

**Globally-scoped** variables are available anywhere in your code, whereas **Locally-scoped** variables are only available within the function they're defined in.

### Scoping can OVERWRITE variables!
---
In the Local scope, you are able to create new variables with the same name as a Globally-scoped variable, without changing or reassigning that value. 

``` javascript
let testVariable = "global";

const testFunction = function() {

  let testVariable = "local";

  console.log("inside testFunction, the testVariable is: " + testVariable);

};

testFunction();

console.log("outside testFunction, the testVariable is " + testVariable);
```
in this example, where a global AND local variable share the same name, the output would be:
``` javascript
inside testFunction, the testVariable is: local
outside testFunction, the testVariable is: global
```

## Best Practice: Pass in Data as Needed
---
Ideally, **the functions in your code should try and avoid reading outer scope variables.** If a function requires data, then it should be passed in as a parameter available within the function's inner (local) scope.

Functions that take in parameters are more reusable, as they're more independent and don't rely on their outer (global) scope.
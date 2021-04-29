# Function Best Practices

## **1. Naming Functions Properly**
The name of your functions directly affect the readability of your code.
* avoid generic function names (data, name, etc.)
* starting function names with verbs (action words) are optimal
* be consistent with your naming conventions
* be mindful and adapt to any existing conventions, esp. when joining existing projects

## **2. Using camelCase**
camelCase is a common JavaScript convention in which every word after the first has the first letter capitalized, and the first word is purely lowercased.

*This does not affect the functionality of your code, but using camelCase is conventional and neater.*

**camelCase examples**: `sayHello`, `createUser`, `sendUserData`

## **3. Proper Indentation**
Indenting your code will make it much easier to read, as you can follow along with the starting points of curly braces and where they end, along with the code within it.

It's conventional to use 2 soft spaces but no tabs.

## **4. Focus on a Single Task**
Single tasks that functions can focus on would ideally be to return a value, or cause a side effect.
You can break your function into additional smaller functions if they do more than one task.

## **5. Pass Necessary Data as Parameters**
If a function requires certain information, it should be passed in as arguments in the local scope rather than being accessed directly. [*Refer to JavaScript Scope for more details.*](/Week_1/Day_2/javascript_scope.md)
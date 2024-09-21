# JavaScript Object Methods

## 1. Object.keys()
- *Purpose*: Returns an array of a given object's own enumerable property names.
- *Returns*: An array of keys.
- *Example*:
    js
    const obj = {a: 1, b: 2, c: 3};
    const keys = Object.keys(obj); // ['a', 'b', 'c']
    

## 2. Object.values()
- *Purpose*: Returns an array of a given object's own enumerable property values.
- *Returns*: An array of values.
- *Example*:
    js
    const obj = {a: 1, b: 2, c: 3};
    const values = Object.values(obj); // [1, 2, 3]
    

## 3. Object.entries()
- *Purpose*: Returns an array of a given object's own enumerable property [key, value] pairs.
- *Returns*: An array of arrays containing key-value pairs.
- *Example*:
    js
    const obj = {a: 1, b: 2, c: 3};
    const entries = Object.entries(obj); // [['a', 1], ['b', 2], ['c', 3]]
    

## 4. Object.assign()
- *Purpose*: Copies the values of all enumerable own properties from one or more source objects to a target object.
- *Returns*: The target object.
- *Example*:
    js
    const target = {a: 1};
    const source = {b: 2};
    const result = Object.assign(target, source); // {a: 1, b: 2}
    

## 5. Object.freeze()
- *Purpose*: Freezes an object, preventing new properties from being added and existing properties from being modified or deleted.
- *Returns*: The frozen object.
- *Example*:
    js
    const obj = {a: 1};
    Object.freeze(obj);
    obj.a = 2; // Error in strict mode, ignored otherwise
    

## 6. Object.seal()
- *Purpose*: Seals an object, preventing new properties from being added, but allows modification of existing properties.
- *Returns*: The sealed object.
- *Example*:
    js
    const obj = {a: 1};
    Object.seal(obj);
    obj.a = 2; // Works
    obj.b = 3; // Fails
    

## 7. Object.create()
- *Purpose*: Creates a new object with the specified prototype object and properties.
- *Returns*: A new object.
- *Example*:
    js
    const proto = {greet: () => console.log('Hello')};
    const obj = Object.create(proto);
    obj.greet(); // 'Hello'
    

## 8. Object.is()
- *Purpose*: Determines whether two values are the same.
- *Returns*: true or false.
- *Example*:
    js
    Object.is(25, 25); // true
    Object.is(NaN, NaN); // true
    Object.is(0, -0); // false
    

## 9. Object.getOwnPropertyDescriptor()
- *Purpose*: Returns an object describing the configuration of a specific property on a given object.
- *Returns*: A property descriptor object.
- *Example*:
    js
    const obj = {a: 1};
    const descriptor = Object.getOwnPropertyDescriptor(obj, 'a');
    // {value: 1, writable: true, enumerable: true, configurable: true}
    

## 10. Object.getPrototypeOf()
- *Purpose*: Returns the prototype of the specified object.
- *Returns*: The prototype of the object.
- *Example*:
    js
    const obj = {};
    const proto = Object.getPrototypeOf(obj); // {}
    

## 11. Object.setPrototypeOf()
- *Purpose*: Sets the prototype of the specified object.
- *Returns*: The object with the new prototype.
- *Example*:
    js
    const obj = {};
    const proto = {greet: () => console.log('Hello')};
    Object.setPrototypeOf(obj, proto);
    obj.greet(); // 'Hello'
    

## 12. Object.fromEntries()
- *Purpose*: Transforms a list of key-value pairs into an object.
- *Returns*: A new object.
- *Example*:
    js
    const entries = [['a', 1], ['b', 2], ['c', 3]];
    const obj = Object.fromEntries(entries); // {a: 1, b: 2, c: 3}
    
"""

# Thank you

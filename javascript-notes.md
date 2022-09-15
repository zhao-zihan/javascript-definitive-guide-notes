## Chapter 2 Lexical Structure

### 1) identifier naming conventions

```javascript
/*
  can use: letters, digits, _, $
  can start with: letters, _, $
*/
```



## Chapter 3 Types, Values, and Variables

### 1) types

```javascript
/*
  primitive (immutable) : number, string, boolean, null, undefined, symbol, bigint
  reference (mutable) : object, functions, arrays
*/
```



### 2) == & ===

```javascript
/*
  == does type conversion
  === compares strictly with no type conversion
  
  0 === -0 is true
  always use ===
*/
```



### 3) .isNaN() & Number.isNaN()

```javascript
/*
	NaN doesn't compare equal to any value including itself

  Number.isNaN() can be replaced by x != x
  Number.isNaN(x) will be true, if and only if x === NaN

  isNaN(x) will be true if x is NaN, or x cannot be converted to a number
*/
```



### 4) why 0.3 - 0.2 = 0.09999999999999998

```javascript
/*
  JavaScript uses IEEE-754 floating-point representation, and it is a binary representation.
  So some values cannot be presented exactly the same as they would be using decimal representation.
  This is called precision lost
*/
```



### 5) BigInt

```javascript
/*
  declaration: 1000n (lowercase)
  conversion: BigInt(x)
  arithmetic: 1000n + 100n
  
  note: 
  100n + 100 will give TypeError
  but comparison operations will give correct answers: 100n > 90 => true
  no Math functions accept BigInt operands
*/
```



### 6) string

```javascript
/*
 1. No char type in js
 2. A unicode character might take up to 2 16-bit values thus has length of 1
 3. for/of loop and ... operator iterate the actual characters rather than 16-bit values
```



### 7) boolean

```javascript
/*
  6 falsy values:
    undefined
    null
    0
    -0
    NaN
    ""
 */
```



### 8) null & undefined

```javascript
/*
  typeof null => object
  typeof undefined => undefined

  undefined === null => false
  undefined == null => true
*/
```



### 9) symbol

```javascript
/*
  declaration: Symbol(x)
  Symbol() function never returns the same value twice even with the exact same input
*/
```


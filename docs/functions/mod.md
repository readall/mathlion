<!-- Note: This file is automatically generated from source code comments. Changes made in this file will be overridden. -->

# Function mod

Calculates the modulus, the remainder of an integer division.

For matrices, the function is evaluated element wise.

The modulus is defined as:

    x - y * floor(x / y)

See http://en.wikipedia.org/wiki/Modulo_operation.


## Syntax

```js
mod(x, y)
```

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
`x` | number &#124; BigNumber &#124; Fraction &#124; Array &#124; Matrix | Dividend
`y` | number &#124; BigNumber &#124; Fraction &#124; Array &#124; Matrix | Divisor

### Returns

Type | Description
---- | -----------
number &#124; BigNumber &#124; Fraction &#124; Array &#124; Matrix | Returns the remainder of `x` divided by `y`.


## Examples

```js
mod(8, 3);                // returns 2
mod(11, 2);               // returns 1

function isOdd(x) {
  return mod(x, 2) != 0;
}

isOdd(2);                      // returns false
isOdd(3);                      // returns true
```


## See also

[divide](divide.md)

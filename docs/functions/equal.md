<!-- Note: This file is automatically generated from source code comments. Changes made in this file will be overridden. -->

# Function equal

Test whether two values are equal.

The function tests whether the relative difference between x and y is
smaller than the configured epsilon. The function cannot be used to
compare values smaller than approximately 2.22e-16.

For matrices, the function is evaluated element wise.
In case of complex numbers, x.re must equal y.re, and x.im must equal y.im.

Values `null` and `undefined` are compared strictly, thus `null` is only
equal to `null` and nothing else, and `undefined` is only equal to
`undefined` and nothing else.


## Syntax

```js
equal(x, y)
```

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
`x` | number &#124; BigNumber &#124; boolean &#124; Complex &#124; Unit &#124; string &#124; Array &#124; Matrix | First value to compare
`y` | number &#124; BigNumber &#124; boolean &#124; Complex &#124; Unit &#124; string &#124; Array &#124; Matrix | Second value to compare

### Returns

Type | Description
---- | -----------
boolean &#124; Array &#124; Matrix | Returns true when the compared values are equal, else returns false


## Examples

```js
equal(2 + 2, 3);         // returns false
equal(2 + 2, 4);         // returns true

var a = unit('50 cm');
var b = unit('5 m');
equal(a, b);             // returns true

var c = [2, 5, 1];
var d = [2, 7, 1];

equal(c, d);             // returns [true, false, true]
deepEqual(c, d);         // returns false

equal(0, null);          // returns false
```


## See also

[unequal](unequal.md),
[smaller](smaller.md),
[smallerEq](smallerEq.md),
[larger](larger.md),
[largerEq](largerEq.md),
[compare](compare.md),
[deepEqual](deepEqual.md)
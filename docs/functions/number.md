<!-- Note: This file is automatically generated from source code comments. Changes made in this file will be overridden. -->

# Function number

Create a number or convert a string, boolean, or unit to a number.
When value is a matrix, all elements will be converted to number.


## Syntax

```js
number(value)
number(unit, valuelessUnit)
```

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
`value` | string &#124; number &#124; BigNumber &#124; Fraction &#124; boolean &#124; Array &#124; Matrix &#124; Unit &#124; null | Value to be converted
`valuelessUnit` | Unit &#124; string | A valueless unit, used to convert a unit to a number

### Returns

Type | Description
---- | -----------
number &#124; Array &#124; Matrix | The created number


## Examples

```js
number(2);                         // returns number 2
number('7.2');                     // returns number 7.2
number(true);                      // returns number 1
number([true, false, true, true]); // returns [1, 0, 1, 1]
number(unit('52cm'), 'm');    // returns 0.52
```


## See also

[bignumber](bignumber.md),
[boolean](boolean.md),
[complex](complex.md),
[index](index.md),
[matrix](matrix.md),
[string](string.md),
[unit](unit.md)

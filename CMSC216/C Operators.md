There are many different operators in C:

## Arithmetic
`+ - * / %` 
- % doesn’t work for floating point (In all cases)
- `/` does truncating integer division when both operands are integers

## Shifting
**Bit Shifting** is when you slide the bits of a value to the left or right
- Left shift (<<) → Bits on left are discarded, 0 bit put on right side
- Right shift (>>) → Adds 0 bits on the right (unless negative it preserves sign then)
- Arrows point towards bit side (The small point)
![[Pasted image 20230307003201.png]]
**Don’t** bit shift negative amounts (undefined so up to compiler)

## Bitwise Operators
`&` → AND (Both need to have 1)
`|` → OR (Either needs to have 1)
`^` → XOR (Only one has one)
Ex: 
```
a = 00101110
b = 01011011
a | b = 01111111
a & b = 00001010
a ^ b = 01110101
```


## Compound Operators
```
+=, -=, *=, /=, %=, <<=, >>=, &=, ^=, |=
```
- Act the same as +=, just wanted to include the others, so I know I can use them

## Unary Operators
`-`  operator → Produces the negative of its operand
`&` operator → Produces memory address of operand
`*` operator → Gets the value of a pointer / memory address
`sizeof` operator → Determines the size of an operator in bytes
	– Can also be used for types `sizeof( int )`
`(type)` operator → Casts the value of expression to another type

## Prefix and Postfix Operators
`++` or `--` can be used before or after the number is returned
- Before the operand → Increments before value is used in expression
- After Operand → Increments after value is used in expression
![[Pasted image 20230307004940.png]]

## Conditional Operator
### `expression1 ? expression2 : expression3`
- `expression1` evaluates first
	– If `expression1` is true, value becomes `expression2`
	– If `expression1` is false, value becomes `expression3`
- Only the correspond one is evaluated
Ex: `a > 5 ? b - 6 : c /2`

### Comma Operator
- Allows you to evaluate things in succession (useful when doing multiple things in a loop)
- Ex: `while( a = get_value(), count_value( a ), a > 0 ) {`
	– Evaluates all arguments, uses the result of the rightmost expression as result

Boolean → *Zero is false, any nonzero value is true*

Important Notes:
- You can only do chained assignments of variables with the same size
- Remember that `&`  and `&&` or `|` and `||` are very different operators

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


## Compound Assignments
```
+=, -=, *=, /=, %=, <<=, >>=, &=, ^=, |=
```
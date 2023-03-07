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

**Don’t** bit shift negative amounts (undefined so up to compiler)




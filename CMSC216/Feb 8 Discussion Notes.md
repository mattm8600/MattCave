## Pipe Operator
In Unix, you can chain together commands in Unix using the `|` operator
Ex:
`display_numbers.x | process_numbers.x`
- Pipes the output of `display_number` to the function `process_numbers` which then uses the output

First thing in Unix is treated as a command

`./executable` means search the current director for `executable`, and if it exists run it

`diff file_1 file_2` → Compares the two files to see if they are the same
- `diff -Y` prints out the files side by side
- allows you to compare two output files and visualize them
- Diff example: `student.x | diff student_expected_values.txt`

`less file_name` → a more versatile way of reading files than cat or something

Literals - Explicitly say what the type is during initialization:
- Ex: `long variable = 3l;` ← Explicitly creates a long
- Ex 2: `unsigned long varialbe = 3u;` ← Creates a positive value (no sign)
- Ex 3: `long variable = 0x30;` ← Hexadecimal number

Binary Addition Algorithm
- Use mod 2 to find that digits number (Ex: 1 + 1 % 2 = 0)
- Use int division by 2 to find carry of number (Ex: 1 + 1 / 2 = 1)
- Use twos-compliment to have a negative number in binary
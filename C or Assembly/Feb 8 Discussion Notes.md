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

`less file_name` → a more versatile way of reading files than cat or something
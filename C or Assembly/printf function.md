Uses a format string and parameters to print something in C

## Syntax:
### `printf(Format str, param1, param2, param3)`
- The format string uses type placeholders to put params into
(insert table of them here)


### Padding
Ex: `printf("%5d", 216)` → Changes the field width to five spaces
- `printf("%05d", 216)` → Fills the five spaces with 0s
- You can use 
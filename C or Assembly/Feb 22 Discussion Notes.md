Best way to do student tests for project:
- Start off running instruction in binary
- Then try to do it in hex

Converting from binary to hex: from left to right, convert each four bits into a binary number
- or use the hex function (should get experience doing it manually though)

raisin-assembler.x → Will make you instructions given a text file Ex: 
``` 
add R2 R3
move R4 R2
sw R4 5600
```

Can’t return void pointers because we don’t know what size they are

Arrays and pointers are virtually the same (they are interchangeable)

`*q--` Returns the current pointer and then decrements
`*++p` Increments then dereferences pointer and returns it


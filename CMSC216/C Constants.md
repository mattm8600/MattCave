Keyword that makes a variable not possible to change
``` 
Ex:
int const a;
const int a;
```

Special Cases with [[Pointers]]:
```
int *pi;
int const *pci;
```
- pci is a pointer to a constant integer
	– You can change the pointer but not the integer it points to

```
int * const cpi;
```
- pci is now a constant pointer to an integer
- pointer’s value cannot change, but you can modify the integer it points to
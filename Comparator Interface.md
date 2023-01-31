**Used to** compare two objects of the same class. External to the objects, we are comparing

### `public int compare(Object obj1, Object obj2)`

Can be used by the Collections `sort()` method
`public void sort(List list, ComparatorClass c)`

Ex:
```
public class sizeComparator implements Comparator<PrinterJob> {

	public int compare(PrinterJob obj1, PrinterJob obj2) {
	return obj1.getSize() - printerJob2.getSize();
	}

}

//To use this in a main method or something:
new SizeComparator().compare(p1,p2);
```
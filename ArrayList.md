# ArrayList

ArrayList is a part of collection framework and is present in java.util package.<br>
It provides us dynamic arrays in Java. <br>

``` Java
import java.util.ArrayList;
import java.util.Collections;

public class Arraylist {

	public static void main(String[] args) {
		
		ArrayList<Integer>arrayList=new ArrayList<Integer>();
		ArrayList<Integer>arrayList1=new ArrayList<Integer>();
		
		arrayList1.add(10);
		arrayList1.add(20);
		arrayList1.add(30);
		arrayList1.add(40);
	
		
		
		arrayList.add(20);
		arrayList.add(10);
		arrayList.add(40);
		arrayList.add(30);
		System.out.println(arrayList);
		
		
		//Printing the element based on the index
		System.out.println(arrayList.get(0));
		
		
		//Sorting the arrayList elements using inbuilt function.
		Collections.sort(arrayList);
		System.out.println(arrayList);
		
		
		//Comparing the arrayLists
		System.out.println(arrayList.equals(arrayList1));
		
		System.out.println(arrayList.contains(300));
		
		
		//Removing the element based on the index.
		arrayList.remove(1);
		
		System.out.println(arrayList);
		
		//Adding the element to a particular index.
		
		arrayList.set(1, 100);
		System.out.println(arrayList);

	}

}


```

# HashSet

It works same as ArrayList.<br>
HashSet doesn't allow duplicate values .<br>
HashSet are not guaranteed to be inserted in the same order<br>


``` java

import java.util.ArrayList;
import java.util.HashSet;
import java.util.Iterator;
import java.util.HashSet;


//Convert Hashset into an Array

public class Hashset {

	public static void main(String[] args) {
		HashSet<Integer> set=new HashSet<Integer>();
		HashSet<ArrayList> hashset=new HashSet<ArrayList>();
		ArrayList<Integer> arrayList=new ArrayList<Integer>();
		ArrayList<Integer> list1=new ArrayList<Integer>();
		ArrayList<Integer> list2=new ArrayList<Integer>();
		
		list1.add(10);
		list1.add(20);
		list2.add(10);
		list2.add(20);
		
		hashset.add(list1);
		
		System.out.println(hashset);
		

		
		
		set.add(10);
		set.add(10);
		set.add(5);
		set.add(3);
		set.add(15);
		set.add(20);
		set.add(20);
		
		//Printing the HashSet
		System.out.println(set);
		
		
		//Iteration over the Hashset.
		Iterator< Integer> it=set.iterator();
		
		Iterator<Integer>it1=set.iterator();
		
		Iterator<Integer>it2=set.iterator();
		
		while(it.hasNext()) {
			arrayList.add(it.next());
		}
		System.out.println(arrayList);
		
		
		
		//Checks weather the set is empty or not.
		System.out.println(set.isEmpty());
		
		
		//deleting an element based on the value
		System.out.println(set.remove(15));
		System.out.println(set);
		
		
		//Printing the size of the hashset.
		System.out.println(set.size());
		
//		System.out.println();
		//Deleting the all the elements of the set.
		set.clear();
	}
}


```


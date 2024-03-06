# Find the second Largest Number in an ArrayList


``` Java
import java.util.ArrayList;

public class SecondLargest {

	public static void main(String[] args) {
		
//		int[] arr= {10,2,4,7,3,9};
		ArrayList<Integer> nums = new ArrayList<Integer>();
		nums.add(1);
		nums.add(2000);
		nums.add(490);
		nums.add(7);
		nums.add(80);
		nums.add(9000);
		
		
		int firstLargest=nums.get(0);
		int secondLargest=nums.get(0);
		
		
		for(int i=1;i<nums.size();i++) {
			
			if(nums.get(i) > firstLargest  ) {
//				
				firstLargest=nums.get(i);
			}
			
		}
		for(int i=0;i<nums.size();i++) {
			if( nums.get(i)>secondLargest && nums.get(i) < firstLargest) {
				secondLargest=nums.get(i);
			}
		}
		
		
		
		System.out.println("The First Largest is "+firstLargest);
		System.out.println("The Second Largest is "+secondLargest);


	}

}


```





# Convert the HashSet into an ArrayList




``` Java
import java.util.ArrayList;
import java.util.HashSet;
import java.util.Iterator;



//Convert Hashset into an Array

public class Hashset {

	public static void main(String[] args) {
		HashSet<Integer> set=new HashSet<Integer>();
		ArrayList<Integer> arrayList=new ArrayList<Integer>();
		set.add(10);
		set.add(10);
		set.add(5);
		set.add(3);
		set.add(15);
		set.add(20);
		set.add(20);

//		System.out.println(set);
		Iterator< Integer> it=set.iterator();

		while(it.hasNext()) {
			arrayList.add(it.next());
		}
		System.out.println(arrayList);

	}
}

```

# Remove Duplicates from an ArrayList


``` java

import java.util.ArrayList;

public class RemoveDuplicates {

	public static void main(String[] args) {
		ArrayList<Integer> nums = new ArrayList<Integer>();
		ArrayList<Integer> num = new ArrayList<Integer>();

		nums.add(12);
		nums.add(2);
		nums.add(2);
		nums.add(9);
		nums.add(9);
		nums.add(10);
//		System.out.println(nums.size());
		
		for(int i=0;i<nums.size();i++) {
			if(num.contains(nums.get(i))) {
//				System.out.println("Push It");
			}
			
			else {
				num.add(nums.get(i));
			}
		}
		
//		for(int i=0;i<num.size();i++) {
//			System.out.println(num.get(i));
//		}
		
		System.out.println(num);

	}

}



```



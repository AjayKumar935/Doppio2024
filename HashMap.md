# HashMap

It provides the basic implementation of the Map interface of Java.<br>
HashMap in Java stores the data in (Key, Value) pairs, and you can access them by an index of another type .<br>
One object is used as a key (index) to another object (value).<br>
If you try to insert the duplicate key in HashMap, it will replace the element of the corresponding key. <br>


``` Java
import java.util.ArrayList;
import java.util.HashMap;

public class Hashmap {

	public static void main(String[] args) {
		
		HashMap<String, Integer> map=new HashMap<String, Integer>();
		ArrayList<String> keys=new ArrayList<String>();
		ArrayList<Integer> values=new ArrayList<Integer>();
		
		map.put("Ajay",100);
		map.put("Anil",200);
		map.put("Abhi",300);
		map.put("Aman",400);
		
		
		//Iteration over the HashMap
		map.forEach((key,value)->{
			System.out.println("Key "+key+" Value "+value);
			
			//Adding the keys to the ArrayList.
			keys.add(key);
			
			//Adding the values to the ArrayList.
			values.add(value)
;		});
		
		
		//Extraction of the value using the key
		System.out.println(map.get("Ajay"));
		
		//Printing the size of the map.
		System.out.println(map.size());
		
		//Printing the Keys
		System.out.println(map.keySet());
		
		//Printing the values
		System.out.println(map.values());
		
		
		
		//Check weather the map is empty or not
		System.out.println(map.isEmpty());
		
		//Updating a value based on a key.
		System.out.println(map.replace("Aman", 700));
		
		System.out.println(map);
		
		
		//Check weather the key is present or not.
		System.out.println(map.containsKey("Ajay"));
		
		//Check weather the value is present or not
		
		System.out.println(map.containsValue(1000));
		
		
		//Printing the keys that are stored in the arrayList
		System.out.println(keys);
		
		
		//Printing the values that are store in the arrayList.
		System.out.println(values);
	

	}

}

```


### Printing the duplicate values using the hashMap


``` java
import java.util.ArrayList;
import java.util.HashMap;

//Find Dupliucates in an arrayMap using a hashmap;



public class DupicatesHashMap {

	public static void main(String[] args) {
		HashMap<Integer, Integer> map=new HashMap<Integer, Integer>();
		ArrayList<Integer> nums = new ArrayList<Integer>();
		
		nums.add(12);
		nums.add(2);
		nums.add(2);
		nums.add(2);
		nums.add(9);
		nums.add(9);
		nums.add(10);
		nums.add(10);
		
		
		for (int i = 0; i < nums.size(); i++) {
            if (map.containsKey(nums.get(i))) {
                map.put(nums.get(i), map.get(nums.get(i)) + 1);
            } else {
                map.put(nums.get(i), 1);
            }
        }

//		map.forEach((key,value)->{
////			System.out.println("Key "+key +" Value " +value);
////			System.out.println("Value " +value);
//
//			if(value>1) {
//				System.out.println(key);
//			}
//		});
		
		map.forEach((key,value)->{
			System.out.println("Key "+key+" Value "+value);
		});

	}

}


```

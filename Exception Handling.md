# Exception Handling <br>
Exception is an event that disrupts the normal flow of the program <br>

# What is Exception Handling 
Exception Handling is a mechanism to handle runtime errors such as ClassNotFoundException, IOException, ArrayIndexOutOfBoundException, NullPointerException etc.

### Types of Java Exceptions
1.Checked Exception  <br>
2.Unchecked Exception <br>

## Checked Exception
Checked exceptions are checked at compile-time <br>

#### Examples
 1.IOException <br> 2.SQLException <br>

 ## Unchecked Exception
 Unchecked exceptions are not checked at compile-time, but they are checked at runtime. <br>
 1.ArithmeticException <br> 2. NullPointerException <br> 3. ArrayIndexOutOfBoundsException <br>

# Keywords used in the exception handling

## try	
The "try" keyword is used to specify a block where we should place an exception code. It means we can't use try block alone. The try block must be followed by either catch or finally. <br>
## catch	
The "catch" block is used to handle the exception. It must be preceded by try block which means we can't use catch block alone. It can be followed by finally block later. <br>
## finally	
The "finally" block is used to execute the necessary code of the program. It is executed whether an exception is handled or not.<br>
## throw	
The "throw" keyword is used to throw an exception. <br>
## throws	
The "throws" keyword is used to declare exceptions. It specifies that there may occur an exception in the method. It doesn't throw an exception. It is always used with method signature. <br>


# ArithmeticException Handling
## Example 1

``` Java
public class ArithmeticException {

	public static void main(String[] args) {
		
		int num=10;
		try {
			System.out.println(num/0);
		}catch(Exception e) {
			System.out.println(e);
		}

	}

}
```

## Output:
``` Java
Exception in thread main java.lang.ArithmeticException:/ by zero
rest of the code...
```

## Example 2

``` Java
import java.math.BigDecimal;

public class ArithmeticException2 {

	public static void main(String[] args) {
		
		BigDecimal i=new BigDecimal(10);
		BigDecimal j=new BigDecimal(3);

		
		try {
			System.out.println(i.divide(j));
		}catch(Exception e) {
			System.out.println(e);
		}
	}

}
```

## Output 

``` Java
java.lang.ArithmeticException: Non-terminating decimal expansion; no exact representable decimal result.
```


# ArrayIndexOutOfBoundException
It Occurs when you try to access the invalid index. <br>

```Java
import java.lang.reflect.Array;

public class ArrayOutOfBound {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int arr[]= {10,20};
		
		try {
			System.out.println (arr[10]);
			
		}catch(Exception e){
			System.out.println (e);
			
			e.printStackTrace();
			System.out.println(e.toString());
			System.out.println(e.getMessage());


			
//			e.toString();
//			e.getMessage();
		}
		

	}

}

```


# NullPointerException
If we have a null value in any variable, performing any operation on the variable throws a NullPointerException. <br>

```Java
public class NullPointerException {

	public static void main(String[] args) {
		
		Object a=null;
		int b=11;
		
		try {
			System.out.println(a.equals(b));
			
//			String s=null;  
//			System.out.println(s.length()); another example
			
		}catch(Exception e) {
			e.printStackTrace();
			System.out.println(e.getMessage());
			System.out.println (e.toString());
		}

	}

}
```

## Output

```Java
java.lang.ArithmeticException: Non-terminating decimal expansion; no exact representable decimal result.

```



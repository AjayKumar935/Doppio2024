# FileReading

``` Java
import java.io.*;
import java.util.*;
public class Read {

	public static void main(String[] args)  {
		
		try {
			File file=new File("input.properties");
			Scanner sc=new Scanner(file);
			
			while(sc.hasNextLine()) {
				String data=sc.nextLine();
				System.out.println(data);
			}
		}catch (Exception e) {
			e.printStackTrace();
		}
		
	}

}

````

## Output

```Java
M3BE.DB.HOST = 13.250.67.210
M3BE.DB.USER = MDBUSR
M3BE.DB.ENV = MVXJDTA
M3BE.DB.DBNAME = M3FDBM3M
M3BE.DB.PWD = Infor2013

```

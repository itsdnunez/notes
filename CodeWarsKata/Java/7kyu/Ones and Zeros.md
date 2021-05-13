## Completion 
Yup 
## Description 
Convert a 4 digit binary number input that is already an array into denary
## My code
```java
import java.util.List;

public class BinaryArrayToNumber {

    public static int ConvertBinaryArrayToInt(List<Integer> binary) {
        int sum = 0;
        int multiplier = 1;
        for (int i = binary.size() - 1; i >= 0; i--){
            sum += multiplier * binary.get(i);
            multiplier *= 2;
        }
        return sum;
      
      /*
      have a sum and a multiplier
      read from the end of the array adding to the sum, the multiplier * 1 or 0 at that point in the array
      double the multiplier each iteration 
      */
    }
}
```
## Better code 
```java
import java.util.List;

public class BinaryArrayToNumber {

    public static int ConvertBinaryArrayToInt(List<Integer> binary) {
        return binary.stream().reduce((x, y) -> x * 2 + y).get();
    }
}
```
## Takeaways 
- existence and usage of lists 
- list.size()
- list.get(x) - access item at x in the list
- binary functions .stream() and reduce() 


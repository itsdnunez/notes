## Completion 
Nope on 12.05.21
## Description 
Check if a string is a valid PIN. A pin is an integer and must be either 4 or 6 digits long. 
## My code
Ha yeah no

## Better code 
```java
import java.util.regex.*;

public class Solution {

  public static boolean validatePin(String pin) {
    return pin.matches("\\d{4}|\\d{6}");
  }

}
```

```java
public class Solution {

  public static boolean validatePin(String pin) {

    if (pin == null || (pin.length() != 4 && pin.length() != 6)) {
      return false;
    }
    
    for (int i = 0; i < pin.length(); i++) {
      if (!Character.isDigit(pin.charAt(i))) {
        return false;
      }
    }
    return true;

  }

}
```
## Takeaways 
 - RTFQ
 - try and catch statements 
 - string.length()
 - Character.isDigit(string)
 - String.charAt(x)
 - Existence of the regex library 


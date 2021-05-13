## Completion

Yup

## Description

Return a reversed string

## My code
```java
public class Kata {

  public static String solution(String str) {
    char[] arr = str.toCharArray();
    String reversed = "";
    for (int x= arr.length - 1; x >=0 ;x--){
      reversed += arr[x];
    }
    return reversed;
  }
}
```
## Better code
```java
public class Kata {

  public static String solution(String str) {
    return new StringBuilder(str).reverse().toString();
  }

}
```

## Takeaways 
str.toCharArray();
StringBuilder functions

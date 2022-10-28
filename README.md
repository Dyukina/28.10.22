# 21.10.22
## 1. Write a function that accepts an integer n and a string s as parameters, and returns a string of s repeated exactly n times.
[Task link](https://www.codewars.com/kata/57a0e5c372292dd76d000d7e/train/java)
___
### Мое рещение 
```java

public class Solution {
    public static String repeatStr(final int repeat, final String string) {
        StringBuilder sb = new StringBuilder();

        for (int i = 0; i < repeat; i++) {
            sb.append(string);
        }

        return sb.toString();
    }
}

```

### Понравившееся решение
```java

class Solution {
  static String repeatStr(int repeat, String string) {
    return string.repeat(repeat);
  }
}

```
## 2. Вам дан массив с положительными числами и неотрицательным числом N. Вы должны найти N-ю степень элемента в массиве с индексом N. Если N находится за пределами массива, то верните значение -1. Не забывайте, что первый элемент имеет индекс 0.
[Task link](https://www.codewars.com/kata/57d814e4950d8489720008db/java)
### Мое рещение 
```java

public class Kata {
  public static int nthPower(int[] array, int n) {
    int result;
    if (array.length > n){
      result = (int) Math.pow (array[n], n);
    }
    else{
      result = -1;
    }
    return result;
  }
}

```

### Понравившееся решение
```java

public class Kata {
  public static int nthPower(int[] array, int n) {
    return n >= array.length ? -1 : (int) Math.pow(array[n], n);
  }
}

```

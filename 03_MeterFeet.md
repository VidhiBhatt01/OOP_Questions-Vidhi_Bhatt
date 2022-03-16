Que: Write a program that reads a number in meters, converts it to feet, and displays the result.

```java
import java.util.Scanner;
class MeterFeet
{
  public static void main(String[] args) 
  {
    Scanner n = new Scanner(System.in);
    System.out.print("Enter Value in Meters :");
    double meter = n.nextDouble();
    double feet = meter * 3.28084;
    System.out.println(meter + " Meters = "+ feet + " Feets");
  }
}

```

Que: Write a program that solves the following equation and displays the value x and y:
1) 3.4x+50.2y=44.5
2) 2.1x+.55y=5.9
(Assume Cramer’s rule to solve equation ax+by=e x=ed-bf/ad-bc cx+dy=f y=af-ec/ad-bc )

```java
import java.util.Scanner;
class CramersRule
{
  public static void main(String[] args) 
  {
    Scanner input = new Scanner(System.in);
    
    System.out.print("Enter value of a : ");
    double a = input.nextDouble();
    
    System.out.print("Enter value of b : ");
    double b = input.nextDouble();
    
    System.out.print("Enter value of e : ");
    double e = input.nextDouble();
    
    System.out.print("Enter value of c : ");
    double c = input.nextDouble();
    
    System.out.print("Enter value of d : ");
    double d = input.nextDouble();
    
    System.out.print("Enter value of f : ");
    double f = input.nextDouble();
    
    double x = ((e*d)-(b*f))/((a*d)-(b*c));
    double y = ((a*f)-(e*c))/((a*d)-(b*c));
    
    System.out.println(x);
    System.out.println(x);
  }
}

```

Que: Write a program that creates a Random object with seed 1000 and displays the first 100 random integers between 1 and 49 using the NextInt (49) method.

```java
import java.util.Random;
class RandomObject
{
    public static void main(String[] args) 
    {
         Random random = new Random(1000);
         for (int i = 0; i < 100; i++) 
        {
            System.out.format("%5d",random.nextInt(49));
            if((i+1)%20==0) System.out.println();
        }
    }
}


```

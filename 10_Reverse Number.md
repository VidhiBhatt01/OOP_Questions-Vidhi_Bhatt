Que: Write a test program that prompts the user to enter ten numbers, invoke a method to reverse the numbers, display the numbers.

```java
import java.util.Scanner;
class ReverseNumber
{
   public static void reverse(int numbers[])
   {
      int j=0,temp;
      
      while(j<=numbers.length/2)
      {
       temp=numbers[j];
       numbers[j]=numbers[numbers.length-1-j];
       numbers[numbers.length-1-j]=temp;
       j++;
      }
   }
   
   public static void main(String[] args) 
   {
      int i=0;
      int num_array[]=new int[5];
      Scanner n = new Scanner(System.in);
      
      for(i=0;i<5;i++)
      {
       System.out.print("Enter at Position "+ (i+1) + " : ");
       num_array[i] = n.nextInt();
      }
      
      reverse(num_array);
      
      System.out.println("After reversing numbers in an Array :"); 
      
      for(i=0;i<5;i++)
      {
       System.out.println("Value at Position "+ (i+1) + " : "+num_array[i]);
      }
   }
}



```

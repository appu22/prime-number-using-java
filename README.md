# prime-number-using-java
Program No 1: Write a program that asks a user to enter an integer n and then determines whether n is prime or not. Your program can perform this by dividing n by all integers from 2 to n-1 and by checking whether the remainder is 0.

 	              
package prime;
import java.util.Scanner;
public class Prime 
{
 public static void main(String[] args) 
{       
 int m=0,flag=0;
 int n=0;
 Scanner in=new Scanner(System.in);
 System.out.println("Enter a number:");
 n=in.nextInt();
 m=n/2;
 if(n==0||n==1)
{
System.out.println(n+"is not prime number");
}
Else
{
 for(int i=2;i<=m;i++)
{
if(n%i==0)
{
flag=1;
break;
}
}
 if(flag==0)
{
 System.out.println(n+"is prime number");  
} 
Else
{
System.out.println(n+"is not prime number");
}
}
}
}



Output1:

Enter a number
5
Given number is prime
BUILD SUCCESSFUL (total time: 2 seconds)

Output2:
Enter a number
6
Given number is not prime
BUILD SUCCESSFUL (total time: 1 second

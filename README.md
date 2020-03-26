# distance-traveled
import java.util.*;

 // Compiler version JDK 11.0.2

 class Dcoder
 {
   public static void main(String args[])
   { 
     int n,evenmulti=1,oddmulti=1,digit;
    Scanner in=new Scanner(System.in);
    System.out.println("enter the distance travelled:");
   n=in.nextInt();
   
   while(n!=0)
   {
     digit=n%10;
     oddmulti=oddmulti*digit;
     n/=10;
     
     if(n==0)
     break;
     
     digit=n%10;
     evenmulti=evenmulti*digit;
     n=n/10;
   }
   if(oddmulti==evenmulti)
   {
     oddmulti=oddmulti*2;
     System.out.println("your bonus is:"+oddmulti);
   }
   else if(oddmulti>evenmulti)
   {
     System.out.println("your bonus is:"+oddmulti);
   }
   else
   {
     System.out.println("your bonus is:"+evenmulti);
   }
   }
 }

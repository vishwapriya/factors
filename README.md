# factors
package com.company;

import java.util.Scanner;

public class Factors {
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int i;
        for(i=2;i<n;i++)
        {
            if(n%i==0)
            {
                if(isprime(i) && i!=1)
                {
                    System.out.print(i);
                    System.out.print(" ");
                }
            }
        }
    }
    public static boolean isprime(int x)
    {
        int j;
        for(j=2;j<=x/2;j++)
        {
            if(x%j==0)
            {
                return false;
            }
        }
        return true;
    }
}

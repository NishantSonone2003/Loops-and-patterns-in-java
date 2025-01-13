# Loops-and-patterns-in-java
1. Rectangular loop

2. import java.util.Scanner;

public class Rectangle {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number of rows");
        int n =sc.nextInt();
        System.out.println("Enter the no of columns");
        int m = sc.nextInt();

        for (int i=1;i<=n;i++){
            for(int j=1;j<=m;j++){
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
if n=5 & m= 4 then output will be  ****
                                   ****
                                   ****
                                   ****
                                   ****

2.Hollow Rectangle
import java.util.Scanner;

public class Hollowrectangle {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Number of Rows");
        int n= sc.nextInt();
        System.out.println("Number of Columns");
        int m=sc.nextInt();

        for(int i=1;i<=n;i++){
            for(int j=1;j<=m;j++){
                if(i==1||j==1||i==n||j==m) {
                    System.out.print("*");
                }
                else{
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
if n=4 and m=5 then output will be *****
                                   *   *
                                   *   *
                                   *****
3.Half Pyramid
import java.util.Scanner;

public class Halfpyramid {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter no of rows");
        int n=sc.nextInt();
//in this code no of rows=no of columns

        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                //no of i=j and cannot exceed i
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
if n=4 then output will be *
                           **
                           ***
                           ****

4.Inverted Half Pyramid
import java.util.Scanner;

public class Invertedhalfpyramid {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter no of rows");
        int n=sc.nextInt();

        for(int i=n;i>=1;i--){
            for(int j=1;j<=i;j++){
                System.out.print("*");
            }

            System.out.println();
        }
    }
}
if n=4 then output will be ****
                           ***
                           **
                           *
5.Half Pyramid but 180°
import java.util.Scanner;

public class Invertedhalfpyramid2 {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter no of rows");
        int n=sc.nextInt();
        //for outer loop
        for(int i=1;i<=n;i++){
            //1st inner loops for space
            for(int j=1;j<=n-i;j++){
                System.out.print(" ");
            }
            //2nd inner loop for *
            for(int j=1;j<=i;j++){
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
if n=4 then output will be     *
                              **
                             ***
                            **** 

6.Number Pyramid

import java.util.Scanner;

public class Numberpyramid {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter no of rows");
        int n=sc.nextInt();

        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                System.out.print(j+" ");
            }
            System.out.println();
        }
    }
}
if n=5 then output will be 1
                           12
                           123
                           1234
                           12345

7.Inverted Number Pyramid
 import java.util.Scanner;

public class InvertedNumberpyramids {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter no of rows");
        int n=sc.nextInt();

        for(int i=n;i>=1;i--){
            for(int j=1;j<=i;j++ ){
                System.out.print(j+" ");
            }
            System.out.println();
        }
    }
}
if n=5 then output will be 12345
                           1234
                           123
                           12
                           1

8.Floyds Triangle

import java.util.Scanner;

public class Floydstriangle {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter no of rows");
        int n=sc.nextInt();
        int number =1;

        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                System.out.print(number+" ");
                number++;
            }
            System.out.println();
        }
    }
}
if n= 5 then output will be 1
                            2 3
                            4 5 6
                            7 8 9 10
                            11 12 13 14 15

9.0-1 triangle 
import java.util.Scanner;

public class Triangle01 {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter the no of rows");
        int n=sc.nextInt();

        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                int sum =i+j;
                if(sum%2==0){
                    System.out.print("1 ");
                }
                else{
                    System.out.print("0 ");
                }
            }
            System.out.println();
        }
    }
}
n=5 then 1
         0 1
         1 0 1
         0 1 0 1
         1 0 1 0 1
                           
                           

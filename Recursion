/*
CSC-239 JAVA
Project Name: Recursion
Student: Weiquan Mai
Date: April 23, 2025
Description: Program utilizes recurison to find the greatest common denominator of two integers.
*/
import java.util.Scanner;

public class Lab18a {
    public static void main(String[] args){
        // Create a scanner
        Scanner input = new Scanner(System.in);

        // Variables
        boolean keepRunning = true;

        // while loop to keep running until q is pressed
        while (keepRunning){
            // Ask user to enter two integers and store integers as string
            System.out.print("Enter two integers (or 'q' to exit): ");
            String buffer = input.nextLine();

            // If string = q, then exit the program
            if(buffer.equalsIgnoreCase("Q")){
            System.out.print("Exiting the program.");
            keepRunning = false;
            break;
           }

            // Else, split string into variables m and n
            String [] variables = buffer.split(" ");
            int m = Integer.parseInt(variables[0]);
            int n = Integer.parseInt(variables[1]);

            // Call gcd method and display results
            System.out.println("The GCD of " + m + " and " + n + " is " + gcd(m,n));
        }

        // CLose scanner
        input.close();
    }
    // Greatest common denominator method
    public static int gcd(int m, int n){
        System.out.println("Entering 'gcd' method: m = " + m +", n = " + n);

        // Base Case
        if (m%n==0){
            System.out.println("Returning 'gcd' value = " + n + " BASE CASE:     m=" + m + ", n=" + n);
            return n;
        }
        // Recursive case
        else{
            int result = gcd(n, m%n);
            System.out.println("Returning 'gcd' value = " + result + "(recursive case: m=" + m + ", n=" + n + ")");
            return result;
        }
    }
}

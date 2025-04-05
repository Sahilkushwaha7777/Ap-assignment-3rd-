# Ap-assignment-3rd-
Class work

# question:-  Write a Program to Print the Pascal's Triangle in Java.


public class PascalTriangle {

    public static void printPascal(int n) {
        for (int line = 0; line < n; line++) {
            int number = 1;

         
            for (int space = 0; space < n - line; space++) {
                System.out.print(" ");
            }

            for (int i = 0; i <= line; i++) {
                System.out.print(number + " ");
                number = number * (line - i) / (i + 1);
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {
        int n = 5; 
        printPascal(n);
    }
}



output:-

     1 
    1 1 
   1 2 1 
  1 3 3 1 
 1 4 6 4 1


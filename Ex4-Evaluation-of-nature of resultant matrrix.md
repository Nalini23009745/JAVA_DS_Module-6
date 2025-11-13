# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE:
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.


## Algorithm

1. Start the program.
2. Read the number of rows and columns for the matrices.
3. Read the elements of Matrix A (all odd numbers).
4. Read the elements of Matrix B (all even numbers).
5. Initialize a result matrix of the same dimension.
6. Add corresponding elements of Matrix A and Matrix B and store in the result matrix.
7. Display the result matrix.
8. Check each element of the result matrix:

   * If all elements are odd, nature = “Odd”
   * If all elements are even, nature = “Even”
   * Otherwise, nature = “Mixed”
9. Display the nature of the resultant matrix.
10. Stop the program.


## Program:
```
/*
Program to ind the nature of resultant matrrix.
Developed by:Nalini P 
RegisterNumber:212223220063
*/

import java.util.Scanner;
public class MatrixAddition{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int rows=sc.nextInt();
        int cols=sc.nextInt();
        int[][] matrixA=new int[rows][cols];
        int[][] matrixB=new int[rows][cols];
        int[][] result=new int[rows][cols];
        for(int i=0;i<rows;i++){
            for(int j=0;j<cols;j++)
            {
                matrixA[i][j]=sc.nextInt();
            }
        }
        for(int i=0;i<rows;i++){
            for(int j=0;j<cols;j++){
                matrixB[i][j]=sc.nextInt();
            }
        }
        for(int i=0;i<rows;i++){
            for(int j=0;j<cols;j++){
                result[i][j]=matrixA[i][j]+matrixB[i][j];
                
            }
        }
        for(int i=0;i<rows;i++){
            for(int j=0;j<cols;j++){
                System.out.print(result[i][j]+" ");
            }
            System.out.println();
        }
        boolean allodd=true;
        outer:
        for(int i=0;i<rows;i++){
            for(int j=0;j<cols;j++){
                if(result[i][j]%2==0){
                    allodd=false;
                    break outer;
                }
            }
        }
        
    }
}

```

## Output:

<img width="866" height="742" alt="image" src="https://github.com/user-attachments/assets/4558899b-8902-4707-b670-7f1a4f4cb0d1" />


## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.

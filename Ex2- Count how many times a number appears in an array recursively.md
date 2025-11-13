# Ex2 Count how many times a number appears in an array recursively.
## DATE:
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm

1. Start the program.
2. Read the number of elements `n` and the array elements.
3. Read the target number to count.
4. Define a recursive function `countOccurrences(arr, n, target)`:

   * Base case: If `n == 0`, return 0.
   * Recursive case:

     * If `arr[n-1] == target`, return `1 + countOccurrences(arr, n-1, target)`.
     * Else, return `countOccurrences(arr, n-1, target)`.
5. Call `countOccurrences(arr, n, target)` and store the result.
6. Display the count of occurrences.
7. Stop the program.


## Program:
```
/*
Program Count how many times a number appears in an array recursively.
Developed by: Nalini P
RegisterNumber: 212223220063
*/

import java.util.Scanner;

public class CountOccurrences {

    public static int countOccurrences(int[] arr, int n, int target) {
        if(n==0)
        return 0;
        if(arr[n-1]==target)
        return 1+countOccurrences(arr,n-1,target);
        else
        return countOccurrences(arr,n-1,target);
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);


        int size = scanner.nextInt();

        if (size <= 0) {
            System.out.println("Invalid array size. Must be positive.");
            return;
        }

        int[] arr = new int[size];
        for (int i = 0; i < size; i++) {
            arr[i] = scanner.nextInt();
        }


        int target = scanner.nextInt();

        int count = countOccurrences(arr, size, target);
        System.out.println("The number " + target + " appears " + count + " time(s) in the array.");

        scanner.close();
    }
}
```

## Output:

<img width="1216" height="735" alt="image" src="https://github.com/user-attachments/assets/c570614e-8329-4d5f-82ef-612c1db4336f" />

## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.

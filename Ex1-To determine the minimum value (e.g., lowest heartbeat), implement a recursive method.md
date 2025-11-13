# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE:
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm

1. Start the program.
2. Read the number of elements `n` and the array elements.
3. Define a recursive function `getMin(arr, i, n)`.
4. Base case: If `i == n-1`, return `arr[i]`.
5. Recursive case: Return the smaller value between `arr[i]` and `getMin(arr, i+1, n)`.
6. Call `getMin(arr, 0, n)` and store the result.
7. Display the minimum value.
8. Stop the program.


## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by:Nalini P
RegisterNumber:212223220063 
*/
```
import java.util.*;

public class Main {
    static int getMin(int[] arr, int i, int n) {
        if (i == n - 1) {
            return arr[i];
        }
        return Math.min(arr[i], getMin(arr, i + 1, n));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.println(getMin(arr, 0, n));
    }
}
```

## Output:

<img width="831" height="382" alt="image" src="https://github.com/user-attachments/assets/933a846b-7394-4029-bf08-5c6735c96caf" />


## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully

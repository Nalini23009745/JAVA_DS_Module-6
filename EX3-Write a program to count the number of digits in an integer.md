# EX3 Write a program to count the number of digits in an integer.
## DATE:
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm

1. Start the program.
2. Read an integer `num` from the user.
3. Initialize a variable `count = 0`.
4. If `num == 0`, set `count = 1`.
5. Otherwise, repeatedly divide `num` by 10 until it becomes 0, incrementing `count` in each step.
6. Display the value of `count` as the number of digits.
7. Stop the program

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by:Nalini P
RegisterNumber:212223220063
*/

import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num=sc.nextInt();
        int count=0;
        int n=num;
        if(n==0)
        {
            count=1;
        }
        else
        {
            while(n!=0){
                n=n/10;
                count++;
            }
        }
      
        
        System.out.println("Number of digits: " + count);
    }
}

```


## Output:

<img width="916" height="387" alt="image" src="https://github.com/user-attachments/assets/a3f0c0f6-0be0-4183-87aa-4c5049f7e726" />


## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.

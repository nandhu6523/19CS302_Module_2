# EX 9 C program to find the sum of odd digits using do while loop.
## DATE:
## AIM:
To write a C program to find the sum of odd digits using do while loop.

## Algorithm
1. Start  
2. Read `num`  
3. Convert `num` to positive if negative  
4. Initialize `sum = 0`  
5. **do-while loop**:  
   - Get last digit  
   - If odd, add to `sum`  
   - Remove last digit  
6. Repeat until `num == 0`  
7. Print `sum`  
8. End   

## Program:
```
#include <stdio.h>
int main() {
    int num, digit, sum = 0;
    scanf("%d", &num);
    if (num < 0) {
        num = -num;
    }
    do {
        digit = num % 10;
        if (digit % 2 != 0) { 
            sum += digit;
        }
        num = num / 10;
    } while (num != 0);
    printf("Sum of odd digits is: %d\n", sum);
    return 0;
}
```

## Output:
![438173364-50700dd8-ea24-45f6-bc58-8ffc4c8d187e](https://github.com/user-attachments/assets/fa6bf9df-6399-4d59-8dbd-f40d90913ef1)



## Result:
Thus the program was executed and the output was verified successfully.

# C-Day-55-Average-of-Numbers
# C Day 55 - Average of Numbers

This program takes multiple numbers from the user, calculates their sum, and finds their average.

## Example Input

```text
Enter how many numbers: 5
Enter number 1: 10
Enter number 2: 20
Enter number 3: 30
Enter number 4: 40
Enter number 5: 50
```

## Output

```text
Sum = 150
Average = 30.00
```

## Concepts Used

* `for` loop
* `scanf()`
* `printf()`
* Variables
* Addition
* Average calculation
* Type casting

## How It Works

1. The program asks how many numbers the user wants to enter.
2. A `for` loop is used to take each number.
3. Every number is added to the `sum` variable.
4. The sum is divided by the total number of values.
5. The average is displayed using two decimal places.

## C Code

```c
#include <stdio.h>

int main()
{
    int n, number;
    int sum = 0;
    float average;

    printf("Enter how many numbers: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++)
    {
        printf("Enter number %d: ", i);
        scanf("%d", &number);

        sum = sum + number;
    }

    average = (float)sum / n;

    printf("Sum = %d\n", sum);
    printf("Average = %.2f", average);

    return 0;
}
```

## Sample Output

```text
Enter how many numbers: 5
Enter number 1: 10
Enter number 2: 20
Enter number 3: 30
Enter number 4: 40
Enter number 5: 50
Sum = 150
Average = 30.00
```

## Goal

The goal of this project is to practice loops, user input, addition, and average calculation in C.

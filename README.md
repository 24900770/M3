 NAME: HARIHARAN M

 REG. NO: 212224100019

# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>

float emi(float p, float r, int t) {
    r = r / (12 * 100);
    return (p * pow(1 + r, t)) / (pow(1 + r, t) - 1);
}

int main() {
    float p, r;
    int t;
    printf("Enter principal, rate, months: ");
    scanf("%f %f %d", &p, &r, &t);
    printf("EMI = %.2f\n", emi(p, r, t));
    return 0;
}

```

## OUTPUT

![image](https://github.com/user-attachments/assets/f97b76c6-9d03-4de1-be89-dedd40a189fa)



## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, a = 0, b = 1, c, i;
    printf("Enter number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci Series: ");
    for(i = 1; i <= n; i++) {
        printf("%d ", a);
        c = a + b;
        a = b;
        b = c;
    }
    return 0;
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/ce8f67bd-5b7c-450b-a3b5-27928112ac7d)

## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i, arr[100];
    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Last element = %d\n", arr[n-1]);
    return 0;
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/11d1ce5d-4616-41a5-aa27-bbc18d752606)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i, x, count = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter %d numbers: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &x);
        if(x % 2 == 0)
            count++;
    }

    printf("Count of numbers divisible by 2 = %d\n", count);
    return 0;
}

```


## OUTPUT

![image](https://github.com/user-attachments/assets/9e71f291-ac47-40a7-a102-ce05e4464851)


## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n, i, arr[100];
    printf("Enter array size: ");
    scanf("%d", &n);

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Updated array: ");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    return 0;
}

```

## Output:
 
![image](https://github.com/user-attachments/assets/2f403f31-1921-4b1e-9242-2b3503106e71)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




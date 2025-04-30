NAME: TAMILSELVAN R

REG NO:212224060275

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


void calculateEMI(float principal, float rate, int time);

int main() {
    float principal, rate;
    int time;

    
    printf("Enter the loan amount (Principal): ");
    scanf("%f", &principal);

    printf("Enter the annual interest rate (in %%): ");
    scanf("%f", &rate);

    printf("Enter the loan duration (in years): ");
    scanf("%d", &time);

    calculateEMI(principal, rate, time);

    return 0;
}


void calculateEMI(float principal, float rate, int time) {
    float monthlyRate;
    int months;
    float emi;

  
    monthlyRate = rate / (12 * 100);
    months = time * 12;

    
    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);

    printf("The EMI is: %.2f\n", emi);
}
```



## OUTPUT
![WhatsApp Image 2025-04-30 at 22 21 56_032efedc](https://github.com/user-attachments/assets/e61e8064-3e48-48f2-871d-b7b03e3b1dce)





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
    int n = 6; 
    int first = 0, second = 1, next, i;

    printf("Fibonacci series for %d terms:\n", n);

    for (i = 0; i < n; i++) {
        if (i == 0)
            next = first;
        else if (i == 1)
            next = second;
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }

    return 0;
}
```
## OUTPUT

![WhatsApp Image 2025-04-30 at 22 22 34_4d1a1f44](https://github.com/user-attachments/assets/fe62ad10-9943-42ca-bd03-7b10caa16f74)







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
    int n, i;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

   
    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
```

## OUTPUT
![WhatsApp Image 2025-04-30 at 22 23 05_f0811bce](https://github.com/user-attachments/assets/f66911c9-3c79-49f3-8f3b-5476986c823e)









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
    int n, i, count = 0;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    
    for (i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```

## OUTPUT

![WhatsApp Image 2025-04-30 at 22 23 39_3bf75c87](https://github.com/user-attachments/assets/bc4dd06d-3c1c-4962-8044-bb548c88bfb0)




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
    int n, i;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    char result[n];

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if (arr[i] % 2 == 0)
            result[i] = 'E';  
        else
            result[i] = '*';  
    }

    printf("Modified array (even replaced with 'E'):\n");
    for (i = 0; i < n; i++) {
        if (result[i] == 'E')
            printf("%c ", result[i]);
        else
            printf("%d ", arr[i]);  
    }

    return 0;
}
```

## Output:
 ![WhatsApp Image 2025-04-30 at 22 24 10_965981c0](https://github.com/user-attachments/assets/85c27ccc-c353-4bbf-920f-1e8efe8a36ab)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




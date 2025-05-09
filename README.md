# EX-11-EMI-CALCULATOR
## REG-NO : 212224040196
## DATE : 27-04-25

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
```c
#include <stdio.h>
#include <math.h>

void calculateEMI(float principal, float annualRate, int months) {
    float monthlyRate = annualRate / (12 * 100);
    float emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);

    printf("The EMI is: %.2f\n", emi);
}

int main() {
    float principal, annualRate;
    int months;

    printf("Enter loan amount (Principal): ");
    scanf("%f", &principal);

    printf("Enter annual interest rate (in percentage): ");
    scanf("%f", &annualRate);

    printf("Enter loan tenure (in months): ");
    scanf("%d", &months);

    calculateEMI(principal, annualRate, months);

    return 0;
}
```


## OUTPUT
![Screenshot 2025-04-27 123210](https://github.com/user-attachments/assets/42d07b15-97a6-4192-8eec-4d475dce8c04)

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
```c
#include <stdio.h>

int main() {
    int n = 6;
    int first = 0, second = 1, next;

    printf("Fibonacci series up to %d terms:\n", n);

    for (int i = 1; i <= n; i++) {
        if (i == 1) {
            printf("%d ", first);
        } else if (i == 2) {
            printf("%d ", second);
        } else {
            next = first + second;
            printf("%d ", next);
            first = second;
            second = next;
        }
    }

    printf("\n");

    return 0;
}

```


## OUTPUT
![Screenshot 2025-04-27 123341](https://github.com/user-attachments/assets/137dcea4-d734-4b7b-9fa5-07a76d7cce0a)


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
```c
#include <stdio.h>

int main() {
    int n;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
```

## OUTPUT

![Screenshot 2025-04-27 123511](https://github.com/user-attachments/assets/16264c35-dd6d-47a3-9583-ad2841f3dece)

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
```c
#include <stdio.h>

int main() {
    int n, count = 0;
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);
    return 0;
}
```


## OUTPUT

![Screenshot 2025-04-27 123755](https://github.com/user-attachments/assets/7ec077cd-9df8-4f17-a873-fc0631fa659d)



## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.


## EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

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
```c
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++){
        scanf("%d",&a[i]);
        if(a[i]%2==0){
            printf("E ");
        }
        else{
            printf("%d ",a[i]);
        }
        
    }
    return 0;
}

```

## Output:

 ![Screenshot 2025-04-27 124601](https://github.com/user-attachments/assets/2ab6ee7d-1042-47a9-b468-2cdec3209834)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




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
void calculateEMI(float principal, float rate, int months) {
    float emi;
    rate = rate / (12 * 100);  
    emi = (principal * rate * pow(1 + rate, months)) / (pow(1 + rate, months) - 1);
    printf("Your EMI is: %.2f\n", emi);
}
int main() {
    float principal, rate;
    int months;
    printf("Enter the principal loan amount: ");
    scanf("%f", &principal);
    printf("Enter the annual interest rate (in percentage): ");
    scanf("%f", &rate);
    printf("Enter the number of months (loan tenure): ");
    scanf("%d", &months);
    calculateEMI(principal, rate, months);
    return 0;
}
```


## OUTPUT
![Screenshot 2025-04-27 000718](https://github.com/user-attachments/assets/97a0c161-33d4-42be-9d30-f1f8c733e5e1)





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
    int n = 6, firstTerm = 0, secondTerm = 1, nextTerm;
    printf("Fibonacci Series up to %d terms:\n", n);
    printf("%d, %d, ", firstTerm, secondTerm);
    for (int i = 3; i <= n; i++) {
        nextTerm = firstTerm + secondTerm;
        printf("%d, ", nextTerm);
        firstTerm = secondTerm;        
        secondTerm = nextTerm;
    }
    printf("\n");
    return 0;
}
```


## OUTPUT
![Screenshot 2025-04-27 000949](https://github.com/user-attachments/assets/d44fedbb-6b43-4c51-a9d6-ca8771df9d0b)



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
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];  
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n-1]);
    return 0;
}
```


## OUTPUT

![Screenshot 2025-04-27 001448](https://github.com/user-attachments/assets/f96abcef-98c3-4398-b4e2-cc0d529a95ef)




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
    int n, count = 0;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("%d\n", count);
    return 0;
}
```




## OUTPUT
![Screenshot 2025-04-27 001909](https://github.com/user-attachments/assets/63e3bff4-236a-4538-b69f-5dd72601a604)



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
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';
        }
    }
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
```


## Output:
![Screenshot 2025-04-27 002334](https://github.com/user-attachments/assets/fa106db2-8e6f-41ee-aff0-eb29260e25f1)

 

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




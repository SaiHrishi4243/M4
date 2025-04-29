# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM

```C

#include <stdio.h>
int main() 
{
    int a = 44,b = 3;
    int result = a << b;
    printf("The result of %d << %d is: %d\n", a, b, result);
    return 0;
}


```
## OUTPUT

![Screenshot 2025-04-30 005401](https://github.com/user-attachments/assets/d89824e6-25f9-4e3c-96cc-155849e0432f)

## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM

```C

#include <stdio.h>
int main() 
{
    int num1, num2;
    printf("Enter the first number: ");
    scanf("%d", &num1);
    printf("Enter the second number: ");
    scanf("%d", &num2);
    if (num1 == num2) 
    {
        printf("Both numbers are equal.\n");
    } 
    else 
    {
        printf("Both numbers are not equal.\n");
    }
    return 0;
}

```

## OUTPUT

![Screenshot 2025-04-30 005551](https://github.com/user-attachments/assets/f11acea9-49bd-419e-be44-8a619ce6cff5)

## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM

```C

#include <stdio.h>
#include <ctype.h>
int main() {
    char str[100];
    int i;
    printf("Enter a string: ");
    scanf("%s", str);
    for (i = 0; str[i] != '\0'; i++) 
    {
        str[i] = tolower(str[i]);
    }
    printf("Lowercase string: %s\n", str);
    return 0;
}

```

## OUTPUT

![Screenshot 2025-04-30 005913](https://github.com/user-attachments/assets/81a30515-3894-4d1a-a5b3-691dcccdb8d7)

## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM

```C

#include <stdio.h>
int main() {
    char str[100];
    int i, count = 0;
    printf("Enter a string: ");
    scanf("%[^\n]", str);
    for (i = 0; str[i] != '\0'; i++) 
    {
        if (str[i] == ' ')
            count++;
    }
    printf("Number of spaces: %d\n", count);
    return 0;
}

```

## OUTPUT

![Screenshot 2025-04-30 010904](https://github.com/user-attachments/assets/effdca09-e187-47fd-a586-af0db4f37808)

## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM

```C

#include <stdio.h>
int main() 
{
    char c1[100], c2[100];
    int flag = 0, i = 0;
    printf("Enter the first string: ");
    scanf("%[^\n]", c1);
    printf("Enter the second string: ");
    scanf("%s", c2);  
    while (c1[i] != '\0' && c2[i] != '\0') 
    {
        if (c1[i] != c2[i]) 
        {
            flag = 1;  
            break;     
        }
        i++; 
    }
    if (flag == 0 && c1[i] == c2[i]) {
        printf("strings are same\n");
    } else {
        printf("strings are not same\n");
    }
    return 0;
}


```

## OUTPUT
 
 ![Screenshot 2025-04-30 011222](https://github.com/user-attachments/assets/9eb07c92-5057-4fea-8338-2644d4376895)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


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
```
#include <stdio.h>

int main() {
    int num = 44; // Integer number
    int shifts = 3; // Number of shifts
    
    // Perform left shift operation
    int result = num << shifts;
    
    // Display the result
    printf("Original number: %d\n", num);
    printf("After left shifting by %d positions: %d\n", shifts, result);
    
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/6de26278-a11c-4ca1-9b5c-bcc33360877d)


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


## OUTPUT
           
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
```
#include <stdio.h>

int main() {
    int num1, num2;
    
    // Input two numbers
    printf("Enter first number: ");
    scanf("%d", &num1);
    
    printf("Enter second number: ");
    scanf("%d", &num2);
    
    // Check if the numbers are equal
    if(num1 == num2) {
        printf("The two numbers are equal.\n");
    } else {
        printf("The two numbers are not equal.\n");
    }
    
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/e4aef182-2f9e-42f1-baf4-484706b4a90f)

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
```
#include <stdio.h>
#include <ctype.h>  // For checking if character is a space

int main() {
    char str[100];
    int i = 0, wordCount = 0;
    
    // Input the string
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin); // Read a line of text including spaces
    
    // Use do-while loop to traverse through the string
    do {
        // If current character is not a space and it is the first character or after a space, it's the start of a word
        if (i == 0 || str[i-1] == ' ') {
            if (str[i] != ' ' && str[i] != '\n' && str[i] != '\0') {
                wordCount++; // Increment word count if it starts a word
            }
        }
        i++; // Move to the next character
    } while(str[i-1] != '\0'); // Loop until the null terminator is reached
    
    // Output the word count
    printf("Total number of words: %d\n", wordCount);
    
    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/5860a386-e690-4c32-b0da-38d11e3e2603)


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
```
#include <stdio.h>

int main() {
    char str1[100], str2[100];
    int i = 0, result = 0;
    
    // Input two strings
    printf("Enter first string: ");
    fgets(str1, sizeof(str1), stdin); // Read the first string
    
    printf("Enter second string: ");
    fgets(str2, sizeof(str2), stdin); // Read the second string
    
    // Compare each character of the strings
    while(str1[i] != '\0' && str2[i] != '\0') {
        if(str1[i] != str2[i]) {
            result = 1; // Strings are not equal
            break;
        }
        i++;
    }
    
    // If the lengths of the strings are different, set result as 1
    if(str1[i] != str2[i]) {
        result = 1;
    }
    
    // Output the result
    if(result == 0) {
        printf("The two strings are equal.\n");
    } else {
        printf("The two strings are not equal.\n");
    }
    
    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/fa87894c-503d-4d21-ad4b-03a1a0e49cea)

 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


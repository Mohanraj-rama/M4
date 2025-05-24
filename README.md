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
    int a = 44;           
    int shift = 3;        
    int result;
    result = a << shift;
    printf("After Left Shift Operation value of a is:%d\n", result);

    return 0;
}
```
## OUTPUT




![image](https://github.com/user-attachments/assets/bce41fe5-61c7-4757-8c2d-34c223c4f973)





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
```
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if(a==b)
    printf("The numbers are equal");
    else
    printf("The numbers are not equal");
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/043fde03-e5d5-4431-99e0-eaf7303d7e5c)
![image](https://github.com/user-attachments/assets/921377fd-cf4b-4743-9372-c910f8e4df4d)

           
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
#include <ctype.h>

int main() {
    char str[100];
    scanf("%s", str);
    int i = 0;
    while (str[i]) {
        str[i] = tolower(str[i]);
        i++;
    }
    printf("Lower case String is:%s\n", str);

    return 0;
}

```

## OUTPUT

![image](https://github.com/user-attachments/assets/6f6ec9be-234d-455c-95ee-1235616e3102)



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

int main() {
    char str[100];
    int i = 0, wordCount = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    do {
        if ((str[i] != ' ' && str[i] != '\n' && str[i] != '\0') && 
            (str[i+1] == ' ' || str[i+1] == '\n' || str[i+1] == '\0')) {
            wordCount++;
        }
        i++;
    } while (str[i] != '\0');

    printf("Total number of words: %d\n", wordCount);
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/e8789b6b-4a2b-4902-95d9-b320d24feca4)




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
#include <string.h>
int compare(char[],char[]);  
int main()  
{  
   char str1[20]; 
   char str2[20];  
   
   scanf("%s",str1);  
    
   scanf("%s",str2);  
   int c= compare(str1,str2);  
   if(c==0)  
   printf("strings are same");  
   else  
   printf("strings are not same");  
  
    return 0;  
}  
  
int compare(char a[],char b[])
{
    int flag=0,i=0;   
    while(a[i]!='\0' &&b[i]!='\0')  
    {  
       if(a[i]!=b[i])  
       {  
           flag=1;  
           break;
       }
       i++;
    }
    if(flag==0)  
    return 0;  
    else  
    return 1;   
}
```

## OUTPUT
 ![image](https://github.com/user-attachments/assets/6c0be691-4327-4fce-8ecc-7c1f4c6afadd)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


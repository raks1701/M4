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
int a = 44, b = 3;
int result;
result = a << b;
printf("Result after left shifting 44 by 3 positions: %d\n",result);
return 0;
}
```
## OUTPUT




![m=1](https://github.com/user-attachments/assets/8dfdaa69-e2db-4b34-94af-f75dffa5ce6b)






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
#include <stdio.h>
int main() {
int num1, num2;
scanf("%d %d", &num1, &num2);
if (num1 == num2) {
printf("Both numbers are equal.\n");
} else {
printf("Both numbers are not equal.\n");
}
return 0;
}
```

## OUTPUT

          

 ![m=2](https://github.com/user-attachments/assets/51c26b1e-b769-441f-b708-ec8577ac8587)

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
int main() {
char str[100];
fgets(str, sizeof(str), stdin);
toLowerCase(str);
printf("Lowercase string: %s\n", str);
return 0;
}
int main() {
char str[100];
fgets(str, sizeof(str), stdin);
toLowerCase(str);
printf("Lowercase string: %s\n", str);
return 0;
}
```
## OUTPUT




![m=3](https://github.com/user-attachments/assets/53b5a77a-a70b-41fb-a98b-0209a0bac538)

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
#include <string.h>
int main() {
char str[100];
int i = 0, wordCount = 0;
fgets(str, sizeof(str), stdin);
str[strcspn(str, "\n")] = '\0';
while (str[i] == ' ') {
i++;
}
do {
if ((str[i] != ' ' && str[i] != '\0') &&
(str[i + 1] == ' ' || str[i + 1] == '\0')) {
wordCount++;
}
i++;
} while (str[i] != '\0');
printf("Total number of words: %d\n", wordCount);
return 0;
}
```
## OUTPUT




![m=4](https://github.com/user-attachments/assets/f7271b7e-ca67-4126-b008-1fd6bf434e31)

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
char c1[100], c2[100];
int i = 0, flag = 0;
scanf("%[^\n]", c1);
getchar();
scanf("%s", c2);
while (c1[i] != '\0' && c2[i] != '\0') {
if (c1[i] != c2[i]) {
flag = 1;
break;
}
i++;
}
if (c1[i] != c2[i]) {
flag = 1;
}
if (flag == 0) {
printf("Strings are same.\n");
} else {
printf("Strings are not same.\n");
}
return 0;
}
```

## OUTPUT

 ![m=5](https://github.com/user-attachments/assets/488cfd8b-6af1-4157-8a60-af8e0d92ff9a)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


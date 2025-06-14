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
#include<stdio.h>
int main(){
    int a=44;
    a=a<<3;
    printf("After Left Shift Operation value of a is:%d",a);
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/9af19e8a-0a23-45f6-89a0-fb6178fe0ea0)










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
    int X, Y;
    scanf("%d", &X);
    scanf("%d", &Y);

    // Check if X and Y are equal
    if (X == Y) {
        printf("X and Y are equal.\n");
    }

    if (X != Y) {
        printf("X and Y are not equal.\n");
    }

    return 0;
}



```


## OUTPUT
![image](https://github.com/user-attachments/assets/96ea91e8-2e08-4b85-b14a-4fd1ff1ef714)

           
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
#include<stdio.h>
#include<ctype.h>
int main()
{
    char str[100];
    scanf("%s",str);
    for(int i=0;str[i] != '\0';i++)
    {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s",str);
    return 0;
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/cf06bbf4-d4f3-4c7b-b75f-74f070d88330)





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
   printf("Enter the string : ");
   scanf("%[^\n]",str);
   int i=0,c=0;
   do{
       if(str[i]==' ') c++;
       i++;
   }while(str[i]!='\0');
   if(str[i]=='\0')c++;
   printf("\nThe total number of words in the given string is: %d",c);
}
```


## OUTPUT
![image](https://github.com/user-attachments/assets/09ad109e-1d0e-4c3a-b4dc-b2f56c272f94)









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
   printf("Enter the string1 : ");
   scanf(" %[^\n]",str1);
   printf("\nEnter the string2 : ");
   scanf(" %[^\n]",str2);
   int s1l=0,s2l=0, f = 0;
   while(str1[s1l]!='\0')s1l++;
   while(str2[s2l]!='\0')s2l++;
   if(s1l==s2l){
      for(int i=0;i<s1l;i++){
          if(str1[i]!=str2[i]){
              f=1;
              break;
          }
      } 
   }
   else f=1;
   if(f==0) printf("\nStrings are same");
   else printf("\nStrings are not same");
  
}

```


## OUTPUT
![image](https://github.com/user-attachments/assets/38bf150b-806c-49b2-88cf-315576c95d85)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


### Name : Muthulakshmi D - 212223040122
# EX-16-LEFT-SHIFT-OPERATION
## AIM
Write a C program to perform the basic left and right shift operation.

## ALGORITHM
1.Input a Number: Read an integer n from the user using scanf.
2.Left Shift Operation: Perform a left shift on n by 2 bits (n << 2) and store the result in variable a.
3.Right Shift Operation: Perform a right shift on n by 2 bits (n >> 2) and store the result in variable b.
4.Display Left Shift Result: Print the value of a after the left shift operation.
5.Display Right Shift Result: Print the value of b after the right shift operation.

## PROGRAM
```
#include <stdio.h>
int main()
{
    int n,a,b;
    scanf("%d",&n);
    a=n<<2;
    b=n>>2;
    printf("After Left Shift Operation value of a is:%d\n",a);
    printf("After Right Shift Operation value of a is:%d",b);
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/75edecc5-d8bf-4650-9f56-bc5d3aa27373)

## RESULT
Thus the program to the basic left and right shift operation with has been executed successfully.


# EX-17- Check Whether a Year Belongs to the 19th Century


## AIM

Write a C program to check whether the entered year is 19th century is valid or not using nested if.

## ALGORITHM
1.Input the Year: Read an integer value from the user and store it in the variable year.
2.Validate the Year: Check if the entered year is greater than or equal to 1000.
3.Check for 19th Century: If valid, check whether the year is between 1900 and 1999 (inclusive).
4.Display Result:
If the year is in the range 1900–1999, print "Year is 19th Century."
Otherwise, print "Year is Not 19th Century."
5.Handle Invalid Year: If the year is less than 1000, print "Invalid Year."


## PROGRAM
```
#include <stdio.h>

int main() {
    int year;
    scanf("%d", &year);

    if (year >= 1000) {
        if (year >= 1900 && year <= 1999) {
            printf("Year is 19th Century.\n");
        } else {
            printf("Year is Not 19th Century.\n");
        }
    } else {
        printf("Invalid Year.\n");
    }

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/f4a887ea-4206-44e2-a6d6-73ff45f01b31)

## RESULT

Thus the program to check whether the entered year is 19th century is valid or not using nested if statement has been executed successfully
 
 


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
int main(){
    char s[100];
    scanf("%s",s);
    int i;
    for(i=0;s[i]!='\0';i++)
    {
        s[i]=tolower(s[i]);
    }
    printf("Lower case String is:%s",s);

    
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/184c4345-c2e9-49eb-8088-e57be90ed899)

## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using for loop.

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
int main()
{
    char s[100];
    scanf("%[^\n]",s);
    int i,count=0;
    for(i=0;s[i]!='\0';i++)
    {
        if((s[i-1]==' ' && s[i]!=' ')||( i==0 && s[i]!=' '))
        count++;
    }
    printf("%d",count);
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/3eeff2d7-7b05-496c-9075-a8cc55738136)

## RESULT
Thus the program to count the total number of words in a given string using for loop has been executed successfully
 
 


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
  
// Comparing both the strings.  
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
 
![image](https://github.com/user-attachments/assets/963e3459-c52c-4259-a9ba-334f8915e643)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


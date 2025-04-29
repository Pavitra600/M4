# EX-16-RIGHT-SHIFT-OPERATION
## AIM
Write a C program to perform the basic right shift operation for 60 integer number with 3 shift. 

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 60 and 3.
3.	Use right shift operator (>>) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    
    int i,num;
    for(i=0;i<60;i++){
        num=i;
    }
    printf("After Right Shift Operation value of a is:%d",num>>3);
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/c7f129f2-c0b3-422b-8d40-dbab0799b361)


## RESULT
Thus the program to perform the basic right shift operation for 60 integer number with 3 shifts has been executed successfully.


 


# EX-17-SMALLEST-AMONG-THREE-NUMBERS


## AIM

C Program to Find the Smallest Number Among Three Numbers

## ALGORITHM

1. Start the program.

2. Read three numbers: a, b, and c.

3. If a is less than both b and c, then a is the smallest.

4. Else if b is less than both a and c, then b is the smallest.

5. Else, c is the smallest.

6. Display the smallest number.

7. Stop the program.
   
## PROGRAM
```
#include <stdio.h>
int main(){
    int a,b,c;
    scanf("%d%d%d",&a,&b,&c);
    if(a<b && a<c){
        printf("%d is the smallest number.",a);
    }
    else if(b<a && b<c){
           printf("%d is the smallest number.",b);
    }
    else{
           printf("%d is the smallest number.",c);
    }
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/f058e602-ca29-4895-b80a-46fd042a8e62)

           
## RESULT

Thus the program to find the smallest among three numbers using simple if statement has been executed successfully
 
 
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
#include <string.h>

int main() {
    char str[100];
    scanf("%s", str);
    for (int i = 0; str[i]; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s\n", str);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/7e02c218-2635-443a-ac8c-dfb22851be64)

## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
write a c program to concatenate without using strcat ,and find the total number of words in a given merged string using Do- while loop.

## ALGORITHM
1. Start the program.

2. Read two string variables, str1 and str2.

3. Concatenate str2 to str1 manually using a loop (without using strcat).

4. Initialize a counter variable wordCount to 1.

5. Initialize index variable i = 0.

6. Use a do-while loop to inspect each character in the merged string:
  If a space ' ' is encountered and the next character is not a space or null, increment wordCount.

7. Continue until the null terminator ('\0') is reached.

8. Display the total number of words.

9. Stop the program.
   
## PROGRAM
```
#include <stdio.h>
#include <string.h>
int main(){
   char str1[100],str2[100],merged[200];
   int i=0,j=0,count=0;
   scanf("%s %s",str1,str2);
   do
   {
       merged[i]=str1[i];
   }while(str1[i++] != '\0');
   i--;
   do{
      merged[i++] = str2[j];
   }while(str2[j++] != '\0');
   i=0;
   do{
       if (merged[i] != '\0')
       count++;
   }while(merged[i++] !='\0');
   printf("%s\n%d",merged,count);
   return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/42d0a93e-71c7-4751-950d-75bf128b87f3)


## RESULT
Thus, the program to concatenate two strings without using strcat() and to count the total number of words in the merged string using a do-while loop has been executed successfully.
 
 


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
int main(){
    char str1[100],str2[100];
    int i=0,count=0;
    fgets(str1,sizeof(str1),stdin);
     fgets(str2,sizeof(str2),stdin);
     
    while(str1[i] != '\0' || str2[i] != '\0'){
        if(str1[i]  != str2[i]){
            count =1;
            break;
        }
        i++;
        
    }
    if(count ==0){
        printf("strings are same");
    }
    else{
        printf("strings are not same");
    }
}
```
## OUTPUT
 ![image](https://github.com/user-attachments/assets/cd7c65a7-1b30-48eb-85c8-8c88dc1a586b)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


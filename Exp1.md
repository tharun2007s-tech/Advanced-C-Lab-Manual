EXP NO:1 C PROGRAM FOR ARRAY OF STRUCTURE TO CHECK ELIGIBILITY FOR THE VACCINE.

Aim:
To write a C program for array of structure to check eligibility for the vaccine person age above 6 years of age.

Algorithm:
1.	Declare structure eligible with age (integer) and n (character array)
2.	Declare variable e of type eligible
3.	Input age and name using scanf, store in e
4.	If e.age <= 6
-	Print "Vaccine Eligibility: No"
Else
-	Print "Vaccine Eligibility: Yes"
5.	Print details (e.age, e.n)
6.	Return 0
 
Program:

```
#include <stdio.h>

struct person {
    int age;
    char name[10];
};

int main() {
    struct person p;
    scanf("%d %s", &p.age, p.name);
    printf("Age:%d\n", p.age);
    printf("Name:%s", p.name);
    printf("vaccine:%d\n", p.age); 
    printf("eligibility:");

    if (p.age > 18) {
        printf("yes");
    } else {
        printf("no");
    }

    return 0;
}
```


Output:

<img width="646" height="311" alt="image" src="https://github.com/user-attachments/assets/8cc61a7a-d394-427a-8706-4daa1ed43a65" />



Result:
Thus, the program is verified successfully. 

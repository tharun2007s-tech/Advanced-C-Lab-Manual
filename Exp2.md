EXP NO:2 C PROGRAM FOR PASSING STRUCTURES AS FUNCTION ARGUMENTS AND RETURNING A STRUCTURE FROM A FUNCTION
Aim:
To write a C program for passing structure as function and returning a structure from a function

Algorithm:
1.	Define structure numbers with members a and b.
2.	Declare variable n of type numbers.
3.	Prompt the user to enter values for a and b.
4.	Input values for a and b into n using scanf.
5.	Call the add function with n as an argument.
6.	Print the result returned by the add function.
7.	Return 0
 
Program:

```
#include <stdio.h>
struct Input
{
    int x;
    int y;
};

struct Output
{
    int sum;
};

struct Output add(struct Input in) 
{
    struct Output out;
    out.sum = in.x + in.y;
    return out;
}

int main() {
    struct Input values;
    struct Output result;
    scanf("%d", &values.x);
    scanf("%d", &values.y);
    result = add(values);
    printf("%d\n", result.sum);

    return 0;
}
```




Output:


<img width="393" height="367" alt="image" src="https://github.com/user-attachments/assets/ef6f7dd1-b656-4293-aa27-251c6b60df47" />





Result:
Thus, the program is verified successfully

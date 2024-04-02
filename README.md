## 1.  write a program that reads input of name and surname and join it with gap.(python,c)

### Python Code 
```
a=input()
b=input()
c=a+' '+b
print(c)
```

### C Code
```
#include <stdio.h>
int main() {
    char a,b[10];
    scanf("%c %s",&a,b);
    printf("%c %s",a,b);
    return 0;
}

```

## 2. swap 2 variables a=22,b=33. (python,c)

###  Python code
```
a=int(input())
b=int(input())
print("Variables before swapping are",a,b)
temp=a  
a=b
b=temp
print("Variables after swapping are",a,b)
```
### C Code
```
#include <stdio.h>
#include<string.h>
int main() {
    char a[20],b[20];
    scanf("%s %s",a,b);
    printf("Variables before swapping are %s %s\n",a,b);
    char temp[20];
    strcpy(temp,a);
    strcpy(a,b);
    strcpy(b,temp);
    printf("Variables after swapping are %s %s",a,b);
    return 0;
}
```
## 3.print a string n times. (ex string=aaa, n = 2 output = aaa aaa). (python,c)
### Python Code
```
a=input()
b=int(input())
c=(a+" ")*b
print(c)
```
### C Code
```
#include <stdio.h>
int main() {
    char a[10];
    int b,i=1;
    scanf("%s %d",a,&b);
    while( i<=b)
    {
        printf("%s ",a);
        i++;
    }
    return 0;
}
```
## 4.

### Python Code
```
a=int(input())
print("Digits before swapping",a)
b=str(a)
s=""
for i in range(len(b)):
    s+=b[len(b)-i-1]
print("Digits after swapping",s)
```

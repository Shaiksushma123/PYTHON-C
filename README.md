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
## 5.

### Python Code
```
# using strlen
a=input()
count=0
for i in range(1,len(a)+1):
    count+=1
print(count)

#  without using strlen
a=input()
count=0
for i in a:
    count+=1
print(count)
```

### C Code
```
#include<stdio.h>
int main()
{
    char a[20];
    int count=0,i;
    scanf("%s",a);
    while(a[i]!='\0')
    {
        count+=1;
        i++;
        
    }
    printf("%d",count);
}
```


## 6.
### Python code
```
a=int(input())
b=int(input())
if (a>b):
    print("a is greater than b")
elif (b>a):
    print("b is greater than a")
else:
    print("a is equal to b")
```

### C Code
```
#include <stdio.h>
int main()
{
    int a,b;
    int greater;
    scanf("%d %d",&a,&b);
    if (a==b)
    printf("%d and %d are equal",a,b);
    else{
    if (a>b) greater=a;
    else if  (b>a) greater=b;
    printf("greater of %d and %d is %d",a,b,greater);
    }
    
}
```

## 7.

### Python Code
```
a=int(input())
b=str(a)
if (b[0]>b[1]):
    greater=b[0]
else:
    greater=b[1]
print("greater of",b[0],"and",b[1],"is",greater)
```
### C
```
#include <stdio.h>
int main()
{
    int a,b,temp,greater;
    scanf("%d",&a);
    temp=a%10;
    b=a/10;
    if (temp>b) greater=temp;
    else greater=b;
    printf("greatest digit of %d is %d",a,greater);
}
```

## 8.
### Python
```
a=input()
b=len(a)
if (a[0]==a[b-1]):
    print("Same")
else:
    print("Not Same")
```
### C
```#include <stdio.h>
#include<string.h>
int main()
{
    char a[20];
    scanf("%s",a);
    int b=strlen(a);
    if (a[0]==a[b-1])
    printf("Same");
    else 
    printf("Not same");
    
}

```


## 9.
### Python
```
a=int(input())
b=str(a)
for i in range(1,len(b)):
    if (int(b[i-1]>b[i])):
        greater=int(b[i-1])
    else:
        greater=int(b[i])
print("greatest digit of",a,"is",greater)
```
### C
```
#include <stdio.h>
int main()
{
    int a,temp;
    int greater=0;
    scanf("%d",&a);
    while(a)
    {
        
        temp=a%10;
        if (temp>greater)
        greater=temp;
        a=a/10;
       
    }
    printf("greatest is %d",greater);
    
}
```
## 10.
### Python
```
a=int(input())
b=str(a)
sum=0
for i in range(0,len(b)):
    sum+=int(b[i])
print(sum)
```
### C
```
#include <stdio.h>
int main()
{
    int a,temp;
    int sum=0;
    scanf("%d",&a);
    while(a)
    {
        
        temp=a%10;
        sum+=temp;
        a=a/10;
        
       
    }
    printf("sum is %d",sum);
    
}
```

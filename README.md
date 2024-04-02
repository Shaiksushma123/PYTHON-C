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

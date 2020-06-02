#include <stdio.h>

int strlength(char mystr[])
{
    int i = 0;
    while (mystr[i] != 0)
    i++;
    
    return i;
}

void append(char *s1, char *s2)
{
      //s2 = s1 + s2;
    int s2len = strlength(s2);
    int s1len = strlength(s1);
    char temp[256] = "";
    for (int i = 0; i <= s1len; i++)
        temp[i] = s1[i];
    for (int i = s1len; i < (s1len + s2len); i++)
        temp[i] = s2[i-s1len];
    for (int i = 0; i <= (s1len + s2len); i++)
        //s2[i] = temp[i];
        s1[i]=temp[i];
}

void inttoroman(int x, char *c)
{
    while (x>=1000){
    x -= 1000;
    append(c, "M");
    }
    while (x>=900){
    x -= 900;
    append(c, "CM");
    }
    while (x>=500){
    x -= 500;
    append(c, "D");
    }
    while (x>=400){
    x -= 400;
    append(c, "CD");
    }
    while (x>=100){
    x -= 100;
    append(c, "C");
    }
    while (x>=90){
    x -= 90;
    append(c, "XC");
    }
    while (x>=50){
    x -= 50;
    append(c, "L");
    }
    while (x>=40){
    x -= 40;
    append(c, "XL");
    }
    while (x>=10){
    x -= 10;
    append(c, "X");
    }
    while (x>=9){
    x -= 9;
    append(c, "IX");
    }
    while (x>=5){
    x -= 5;
    append(c, "V");
    }
    while (x>=4){
    x -= 4;
    append(c, "IV");
    }
    while (x>=1){
    x -= 1;
    append(c, "I");
    }
    while (x = 0)
    append(c, "0");
}

int main()
{
    int x;
    char c[256];
    
    printf("enter integer to be converted to roman numerals: \n");
    scanf("%d", &x);
    
    if (x > 1)
    {
        inttoroman(x, c);
        printf("the converted value is %s", c);
    }
    else
        printf("the converted value is 0");
    return 0;
}




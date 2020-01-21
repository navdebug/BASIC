#include<stdio.h>
void function()
{
    char r;
    scanf("%s",&r);
    //return r;
    if(r=='a'||r=='e'||r=='i'||r=='o'||r=='u')
    printf("VOWEL");
    else
    printf("CONSONANT");
}
int main()
{
    function();
}

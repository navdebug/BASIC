# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
#include<string.h>

int main(){
  int t;
  scanf("%d",&t);
  while(t--){
    int n,d,i,j;
    scanf("%d %d",&n,&d);
    char a[100001],b[n+1];
    scanf("%s%s",a,b);
    char t='a';
    
    for (i=0;i<strlen(a);i++){
      if (b[i]!=a[i]){
        j=i+d;
        while(j<n){
          if(a[i]==b[j]){
            t=b[i];b[i]=b[j];b[j]=t;
          }
          j=j+d;
        }
      }
    }
    if (strcmp(a,b)==0){
      printf("Yes\n");
    }
    else{
      printf("No\n");
    }
  }
  return 0;
}

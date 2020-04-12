# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
#include<stdlib.h>

int scanint();

int main(){
	int t=scanint();
	int n;
	int *a;
	int flag;
	int temp;
	for(int i=0;i<t;i++){
		flag=1;
		n=scanint();
		a=malloc(sizeof(int)*n);
		for(int j=0;j<n;j++)
			a[j]=scanint();
		for(int j=0;j<n-1;j++){
			if(a[j]>a[j+1]){
				temp=a[j];
				a[j]=a[j+1];
				a[j+1]=temp;
				j++;
			}
		}
		for(int j=0;j<n-1;j++)
			if(a[j]>a[j+1]){
				flag=0;
				break;
			}
		if(flag)
			printf("YES\n");
		else
			printf("NO\n");
	}
}

int scanint(){
	char c=getchar_unlocked();
	while(c<'0' || c>'9')
	c=getchar_unlocked();
	int x=0;
  	while(c>='0' && c<='9'){
		x=(x<<1)+(x<<3)+c-48;
		c=getchar_unlocked();
	}
	return x;
}

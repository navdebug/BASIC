#include<stdio.h>
int main()
{
	
	scanf("%d",&t);
	
	while(t--){
	    char input[10000];
	    
	    int upper = 0;
	    int lower = 0;
	    int num = 0;
	    int others = 0;
	    
	    scanf("%s",input);
	    
	    for(int i = 0; i < strlen(input);i++){
	        if(input[i] >= 'A' && input[i] <= 'Z'){
	            upper++;
	        }
	        else if(input[i] >= 'a' && input[i] <= 'z'){
	            lower++;
	        }
	        else if(input[i] >= 48 && input[i] <= 57){
	            num++;
	        }
	        else {
	            others++;
	        }
	    }
	    
	    printf("%d\n%d\n%d\n%d\n",upper,lower,num,others);
	}
	
	return 0;
}

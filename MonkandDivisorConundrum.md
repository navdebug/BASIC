# BASIC
CodeChef Programs at beginner and easy level
int main() {
 
int n,p,q,a,b,c;
scanf("%d",&n);
int arr[n];
for(int i=0;i<n;i++){
    scanf("%d",&arr[i]);
}
int test_case;
scanf("%d",&test_case);
while(test_case>0){
    scanf("%d%d",&p,&q);
     a=0,b=0,c=0;
    for(int i=0;i<n;i++){
       
        if(arr[i]%p==0)
        a++;
        if(arr[i]%q==0)
        b++;
        if(arr[i]%p==0 && arr[i]%q==0)
        c++;
    }
    printf("%d\n",a+b-c);
    test_case--;
}
return 0;
}

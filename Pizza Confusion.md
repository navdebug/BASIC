# BASIC
CodeChef Programs at beginner and easy level
    #include<string.h>
    #include<stdio.h>
    int main()
    {
        int n;
        scanf("%d",&n);
        long long  int p,p1;
        char s[21],s1[21];
        scanf("%s%d",s,&p);
        for(int i=0;i<n-1;i++)
        {
            scanf("%s%d",s1,&p1);
            if(p<p1)
            {
                p=p1;
                strcpy(s,s1);
            }if(p==p1)
            {
                 p=p1;
                if(strcmp(s,s1)>0)
                    strcpy(s,s1);
            }
        }
        printf("%s",s);
     
        return 0;
    }

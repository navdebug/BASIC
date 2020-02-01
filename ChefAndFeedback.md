#include <stdio.h>
#include <string.h>

int main() {

	int t;
	scanf("%d", &t);

	while(t--) {

          char str[600005];
          int len, flag = 0;

          for (int i = 0; i < 600005; i++) {
               str[i] = 0;
          }

          scanf("%s", str);

          len = strlen(str);

          for (int j = 0; j < len - 2; j++) {
               if (str[j] == '1' && str[j+1] == '0' && str[j+2] == '1') {
                    flag = 1;
                    break;
               }
               else if (str[j] == '0' && str[j+1] == '1' && str[j+2] == '0') {
                    flag = 1;
                    break;
               }
          }

          if (flag) {
               printf("Good\n");
          }
          else {
               printf("Bad\n");
          }
          }
          }

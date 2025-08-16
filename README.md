// Online C compiler to run C program online
#include <stdio.h>
int primenumber(int n);
int main(){
int num,flag=0;
printf("enter a number: ");
scanf("%d",&num);
flag=primenumber(num);
if(flag==1){
printf("%d is not a prime number",num);
}
else{
printf("%d is a prime number",num);}
return 0;
}
int primenumber(int n){
   int flag=0; 
for(int i=2;i<=n/2;i++){
if(n%i==0){
flag=1;
break;}
}
return flag;
}



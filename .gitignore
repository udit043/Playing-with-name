#include <iostream.h>
#include <windows.h>
#include <stdio.h>

using namespace std;

void swap(char *p,char *q)
   {
    char c;
    c=*p;
    *p=*q;
    *q=c;
   }

void perm(char *a,int m,int n)
  {
   int r; 
   if (m == n)
    {
     printf("%s\n", a);
    }
   else
    {
     for (r = m; r <= n; r++)
      {
        swap((a+m), (a+r));
        perm(a, m+1, n);
        swap((a+m), (a+r)); //backtrack
      }  
    }
  }

int main(int argc, char *argv[])
{
   char a[80],rev[80];
   int i,j,l,flag=1,e,f,g,k; 
     
   system("title Udit Raikwar Program by using C++");
   cout<<"Enter your name : ";
   gets(a);
   for(e=0;a[e]!=0;++e);
   Sleep(1200);
   cout<<"Number of words in your name : ";
   Sleep(800);
   cout<<e;
   f=e-1;
   Sleep(1200);
   cout<<"\nMaking reverse of your name : ";   
   for(l=0,f=e-1;f>=0;++l,--f)
   {
   rev[l]=a[f];
   }
   rev[l]='\0';  //for null character
   Sleep(1200);
   puts(rev);
   Sleep(1200);
   cout<<"Checking condition for palindrome : \n\n";
   Sleep(1200);

     if(strcmp(a,rev)==0)
     {
       flag=2;
     }
     else
     {
       flag=0;
     }
   
   if(flag==2)
   {
     cout<<"palindrome\nOnly one arrangment is possible (i.e. original string) : ";
     puts(a);
     cout<<endl;
   }
   else if(flag==0)
   {
     cout<<"Not Palindrome\n";
     Sleep(1200); 
     cout<<"All possible combinations :\n";
     Sleep(1200);
     cout<<"Wait for a  second ..\n";
     Sleep(1200);
     j=strlen(a);
     k=1;
     for(i=j;i!=0;--i)
     {
       k*=i;
     }
     cout<<"\nYour name can be arrange in ";
     cout<<k;
     cout<<" ways\n";
     cout<<"\nDo you want to see combinations of all your naming words , press \n1 for Yes\n2 for No\n";
     cin>>g;
     if(g==1)
     {
       cout<<endl;
       perm(a,0,strlen(a)-1);
     }
     else
     {
       cout<<"bye..\n";
       Sleep(1200);
     }
   } 
    system("pause");
    return EXIT_SUCCESS;    
}

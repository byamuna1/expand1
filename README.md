#include <iostream>
using namespace std;
void fun(char c,char s[],int x)
{
    int y=0;
    while(s[x]>='0'&&s[x]<='9')
    {
        
            y=(y*10)+(s[x]-48);
            x++;
    }
    for(int i=1;i<=y;i++)
    cout<<c;
}

int main() {
    int t;
    cin>>t;
    while(t-->0)
    {
        char a[1000];
        cin>>a;
        for(int i=0;a[i]!='\0';i++)
        {
            if((a[i]>='a'&&a[i]<='z')||(a[i]>='A'&&a[i]<='Z'))
            {
                fun(a[i],a,i+1);
            }
        }
        cout<<endl;
    }
    
}	


#include<iostream>
#include<stdio.h>
#include<algorithm>
#include<math.h>
#define INF 1000000

using namespace std;

double a[3],ans;
char x,y;

double cal(double a1,double a2,char c)
{
    if(c=='+')return a1+a2;
    if(c=='-')return a1-a2;
    if(c=='*')return a1*a2;
    if(c=='/'&&a2!=0)return a1/a2;
    else if(c=='/'&&a2==0)return INF;
}

int main()
{
    double temp;
    for(int i=0;i<30;i++)
    {
        scanf("%lf",&a[0]);
        scanf("%c",&x);
        scanf("%lf",&a[1]);
        scanf("%c",&y);
        scanf("%lf",&a[2]);
        if((x=='+'||x=='-')&&(y=='*'||y=='/'))
        {
            temp=cal(a[1],a[2],y);
            ans=cal(a[0],temp,x);
        }
        else
        {
            temp=cal(a[0],a[1],x);
            ans=cal(temp,a[2],y);
        }
        if(ans>=0&&ans<=100)printf("%lf\n",ans);
        else printf("No Answer\n");
    }
    return 0;
}

# TheNeverless.github.io
#include 
using namespace std;
int main()
{
    int n,m,p;
    scanf("%d%d%d",&n,&m,&p);
    int a[n],b[n];
    double c[n];
    int i;
    for(i=0;i<n;i++)
    {
        scanf("%d%d",&a[i],&b[i]);
    }
    for(i=0;i<n;i++)
    {
        c[i] = a[i]*0.85+b[i]*0.15;
    }
    sort(c,c+n);
    double x;
    x = (c[n-m]-0.15*p)/0.85;
    if(x<0)
        printf("0");
   else printf("%.0f",ceil(x));
    return 0;
}

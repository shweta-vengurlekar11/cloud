**calling display 1 function from display 2**

```
#include<iostream>
using namespace std;

class myclass1
{
public:
void disp1()	
{
cout<<"in disp 1"<<endl;
}
};

class myclass2
{
public:
void disp2(myclass1 &ref)	
{  
cout<<"in disp 2"<<endl;		
ref.disp1();	
}
};
int main()
{
myclass2 m2;
myclass1 m1;
m2.disp2(m1);
return 0;

}
```

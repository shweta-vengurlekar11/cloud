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

output:

![image](https://user-images.githubusercontent.com/63588827/80831087-c9694300-8c07-11ea-9d95-0c18a59d3e95.png)

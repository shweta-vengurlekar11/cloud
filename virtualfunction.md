**virtual function example**

```
#include<iostream>
using namespace std;

class myclass1
{
public:
	myclass1() {}
	virtual void function()
	{
		cout << "in myclass1" << endl;
	}
}
;
class myclass2 :public myclass1
{
public:
	myclass2() {}
	void function()
	{
		cout << "in myclass2" << endl;
	}
	};

int main()
{
	myclass1 m;
	m.function();
	myclass2 m1;
	myclass1 *m2 = &m1;
	m2->function();
}
```

output:

![image](https://user-images.githubusercontent.com/63588827/80831243-09c8c100-8c08-11ea-9560-fa82f1c99a6d.png)

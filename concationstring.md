**string concatanation**

```
#include<iostream>
#include<string.h>
using namespace std;
class  Second;
class First
{
	char str1[20];
	friend void concat(First&, Second&);
public:
	First(char str[])
	{
		strcpy(str1, str);
	}
};
class Second
{
	char str2[20];
	friend void concat(First&, Second&);
public:
	Second(char str[])
	{
		strcpy(str2, str);
	}
};

void concat(First& f, Second& s)

{
	cout << strcat(f.str1, s.str2)<<endl;
};
int main()
{
	First f("hello");
	Second s("world!");
	concat(f, s);
	return 0;
}
```

output:

![image](https://user-images.githubusercontent.com/63588827/80831406-62985980-8c08-11ea-8e08-0af691095244.png)

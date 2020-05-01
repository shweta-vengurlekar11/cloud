**fibonacci series**

```
#include <iostream>
using namespace std;

int main()
{
    int n, t1 = 0, t2 = 1, nextTerm = 0;

    n = 10;
    cout << "Fibonacci Series: ";

    for (int i = 1; i <= n; ++i)
    {
        if (i == 1)
        {
            cout << t1<<" ";
            continue;
        }
        if (i == 2)
        {
            cout << t2 << " ";
            continue;
        }
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;

        cout << nextTerm << " ";
    }
   cout<<endl;
 return 0;
}
```

output:

![image](https://user-images.githubusercontent.com/63588827/80831653-d9cded80-8c08-11ea-99c0-55f8534e2e66.png)

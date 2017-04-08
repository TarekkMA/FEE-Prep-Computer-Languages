## Chapter 4 Answers
***
** Questions index: **    
[1](#1) . [2](#2) . [3](#3) . [4](#4) . [5](#5) . [6](#6) . [7](#7) . [8](#8) . [9](#9) . [10](#10) . [11](#11) . [12](#12) . [13](#13) . [14](#14) . [15](#15) . [16](#16) . [17](#17) . [18](#18)
***
#### 1   
```cpp
y % 4 == 0 && (y % 100 != 0 || y % 400 == 0)
```
#### 2
```cpp
void addOneRed(int &x){
    ++x;
}
int addOneVal(int x){
    return ++x;
};
```
#### 3
```cpp
#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    float x = 1.04719755;// = pi/3
    float lhs = cos(2*x);
    float rhs = 2 * pow(cos(x),2) - 1;
    if(lhs == rhs){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}

```
#### 4
```cpp
#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    float x = 1.04719755;// = pi/3
    float result = pow(cos(x),2) + pow(sin(x),2);
    if(result == 1){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 5

```cpp
#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    float x = 52.56;
    float b = 12;

    float rhs = pow(b,x);
    float lhs = pow(exp(1),x * log(b));

    if(lhs == rhs){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 6
```cpp
#include <iostream>

using namespace std;

int min(int n1,int n2,int n3,int n4){
    int curMin = n1;
    if(curMin > n2)curMin = n2;
    if(curMin > n3)curMin = n3;
    if(curMin > n4)curMin = n4;
    return curMin;
}

int main()
{
    int n1 = 6,
        n2 = -3,
        n3 = 1,
        n4 = 10;


    if(min(n1,n2,n3,n4) == -3){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 7
```cpp
#include <iostream>

using namespace std;

int max(int n1,int n2){
    int curMax = n1;
    if(curMax < n2)curMax = n2;
    return curMax;
}
int max(int n1,int n2,int n3,int n4){
    return max(max(n1,n2),max(n3,n4));
}


int main()
{
    int n1 = 6,
        n2 = -3,
        n3 = 15,
        n4 = 10;


    if(max(n1,n2,n3,n4) == 15){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 8
```cpp
#include <iostream>

using namespace std;

int min(int n1,int n2){
    int curMin = n1;
    if(curMin > n2)curMin = n2;
    return curMin;
}
int min(int n1,int n2,int n3,int n4){
    return min(min(n1,n2),min(n3,n4));
}


int main()
{
    int n1 = 6,
        n2 = -3,
        n3 = 15,
        n4 = 10;


    if(min(n1,n2,n3,n4) == -3){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 9
```cpp
#include <iostream>

using namespace std;

float average(float x1,float x2,float x3,float x4){
    return (x1+x2+x3+x4)/4.0;
}


int main()
{
    int n1 = 6,
        n2 = -3,
        n3 = 15,
        n4 = 10;


    if(average(n1,n2,n3,n4) == 7){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```

#### 10
```cpp
#include <iostream>

using namespace std;

float average(float x1,float x2=0,float x3=0,float x4=0){
    float number = 1;
    if(x2!=0)number++;
    if(x3!=0)number++;
    if(x4!=0)number++;
    return (x1+x2+x3+x4)/number;
}


int main()
{
    int n1 = 6,
        n2 = -3,
        n3 = 15,
        n4 = 10;


    if(average(n1,n2,n3,n4) == 7 && average(n3,n4) == 12.5){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 11

```cpp
#include <iostream>

using namespace std;

int fact(int n){
    int f=1;
    for(int i=1;i<=n;i++){
        f*=i;

        if(f<0) // !!! integer overflow !!!
            return -1;  // exit the function returing -1
    }
    return f;
}

int main()
{
    int a = 15;
    int af = fact(a);
    int b = 60;
    int bf = fact(b);

    if(af!=-1)cout << a << "! = " << af << endl;
    else cout << a << "! Overflows !" << endl;

    if(bf!=-1)cout << b << "! = " << bf << endl;
    else cout << b << "! Overflows !" << endl;

    return 0;
}
```
#### 12
```cpp
#include <iostream>

using namespace std;

int perm(int n,int k){
    //nPk = (n!) / (n-k)!
    int p = 1;
    for (int i=n;i>(n-k);i--){
        p*=i;
    }
    return p;
}

int main()
{
    int n=5,k=3;
    if (perm(n,k) == 60){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```

#### 13
```cpp
#include <iostream>

using namespace std;

int fact(int n){
    int f=1;
    for(int i=1;i<=n;i++)f*=i;
    return f;
}

int comp(int n,int k){
    //nCk = (n!) / k! * (n-k)!
    int c = fact(n) / (fact(k) * fact(n-k));
    return c;
}

int main()
{
    int n=6,k=3;
    if (comp(n,k) == 20){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 14
```cpp
#include <iostream>

using namespace std;

int fact(int n){
    int f=1;
    for(int i=1;i<=n;i++)f*=i;
    return f;
}

int perm(int n,int k){
    //nPk = (n!) / (n-k)!
    int p = 1;
    for (int i=n;i>(n-k);i--){
        p*=i;
    }
    return p;
}

int comp(int n,int k){
    //nCk = nPk / k!
    int c = perm(n,k)/fact(k);
    return c;
}

int main()
{
    int n=6,k=3;
    if (comp(n,k) == 20){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 15
```cpp
#include <iostream>
#include <cmath>

using namespace std;

int digit(int n,int k){
    int number1 = n * pow(10,-k);
    int result = number1%10;
    return result;
}

int main()
{
    int n=29415,k1=3,k2=0,k3=1;
    if (digit(n,k1)==9 && digit(n,k2)==5 && digit(n,k3)==1){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 16
```cpp
#include <iostream>

using namespace std;

int gcd(int number1,int number2){
    int number = number1;
    int divisor = number2;
    int reminder = number%divisor;
    while(reminder != 0){
        number = divisor;
        divisor = reminder;
        reminder = number%divisor;
    }
    return divisor;
}

int main()
{
    if (gcd(216,594) == 54 && gcd(216,594)==gcd(594,216)){
        cout << "PASS\n";
    }else{
        cout << "FAIL\n";
    }
    return 0;
}
```
#### 17
```cpp
#include <iostream>

using namespace std;

double power(double x,int p){
    double result=1;
    for (int i = 1;i<=p;i++)result*=x;
    return result;
}

int main()
{
    if (power(2,3)==8 && power(2,20)==1048576){
        cout << "TEST PASS\n";
    }else{
        cout << "TEST FAIL\n";
    }

    int x = 2;
    cout << x << "^20 = " << power(x,20) << endl;

    return 0;
}
```
#### 18

```cpp
#include <iostream>
#include <cmath>

using namespace std;

int isSquare(int x){
    float sqrtx = sqrt(x);
    if(sqrtx > (int)sqrtx){
         return 0; // FALSE
    }else{
        return 1; // TRUE
    }
}

int main()
{
    if (isSquare(4) && !isSquare(10) && isSquare(64) && !isSquare(70)){
        cout << "TEST PASS\n";
    }else{
        cout << "TEST FAIL\n";
    }
    return 0;
}
```

# 2012 Final
---
## Page 1
![p1](page1.jpg)
## Page 2
![p1](page2.jpg)

## 2-3
![p1](q3.jpg)

```cpp
float mark;

	do{
		cout << "Please enter the mark should be between 0 and 100:";
		cin >> mark;
	}while(mark > 100||	mark < 0);
```

## 2-4
![p1](q4.jpg)
```cpp
for(int i=51;i<100;i+=2) cout << i << endl;
```

## 3
![p1](q3-1.jpg)
```cpp
#include <iostream>

using namespace std;


int main(){

	float sum = 0;
	int n;
	cout << "Enter number: ";
	cin >> n;

	for(int i = 1;i<=n;i++) sum += (1.0/i) ;

	cout << "Sum is " << sum << endl;

}
```

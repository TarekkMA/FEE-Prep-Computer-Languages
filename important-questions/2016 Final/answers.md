# 2016 Final
---
## ** 2 **

###  a
![a](1-a.jpg)
```
5
-10
```
###  b
![b](1-b.jpg)
```
11
```
###  c
![c](1-c.jpg)
```
-27
```
###  d
![d](1-d.jpg)
```
7
```
###  e
![e](1-e.jpg)
```
A
```
###  f
![f](1-f.jpg)    
** سؤال مقطوش :\ **   
** هنعتبر البرنامج نادي الفانكشن وطلع الخرج ع الشاشة **

```
sum(x,y,z) = 13
الخرج
13
```
## **3**
### a
![](2-a.jpg)
```cpp
	do{
		cout << "Enter N:";
		cin >> n;
	}while(n<30);

	for(int i=6;i<n;i+=2) cout << i << endl;
```
### b
![](2-b.jpg)
```cpp
	int sum = 0;

	int i = 200;

	do{
		if(i%7==0) sum+= i;
	}while(++i<=300);

	cout << "Sum is " << sum << endl;
```
### c
![](2-c.jpg)
```cpp
	int n;

	do{
		cout << "Enter Number: ";
		cin >> n;
		if(n<0) cout << n << " is a negative number !\n";
	}while(n!=0);
```
### e
![](2-e.jpg)
```cpp
const int arrLen = 5;
int arr[arrLen] = {5,10,15,20,25};

for(int i=arrLen-1 ; i>=0 ; i--)
  cout << arr[i] << endl;
```
### f
![](2-f.jpg)
```cpp
const int STUDENTS_NUM = 25;
float x[STUDENTS_NUM];

for(int i = 0;i<STUDENTS_NUM;i++){
  cout << "Enter grades for student #" << i+1 << ":";
  cin >> x[i];
}
```

## **3**

### a
![](3-a.jpg)
```cpp
return_type name(pram_type param_name){
  boady
}
```
### b
![](3-b.jpg)
```cpp
#include <iostream>

using namespace std;

long Fact(int n){
	if(n<=1)return 1;
	else return n * Fact(n-1);
}

int main(){

	int num;
	cout << "Enter Number:";
	cin >> num;

	cout << num << "! = " << Fact(num) << endl;


}
```
### c
![](3-c.jpg)
```cpp
#include <iostream>

using namespace std;

int Min(int arr[],int size){
	int min = arr[0];
	for(int i=1;i<size;i++){
		if(arr[i] < min) min = arr[i];
	}
	return min;
}

int main(){

	int n;
	cout << "Enter Number:";
	cin >> n;

	int arr[n];

	for(int i=0;i<n;i++){
		cout << "Enter Number " << i+1 << ":";
		cin >> arr[i];
	}

	cout << "The min is " << Min(arr,n) << endl;


}
```
## **4**

### a
![](4-a.jpg)
```cpp
type name[length];
```
### b
![](4-b.jpg)
```cpp
#include <iostream>

using namespace std;

int main(){

	const int ARR_SIZE = 30;
	int A[ARR_SIZE];

	int count = 0;

	for(int i=0;i<ARR_SIZE;i++){
		cout << "Enter #"<<i+1<<": ";
		cin >> A[i];
		if(A[i]%2!=0)count++;
	}

	cout << "Array :\n";
	for(int i=0;i<ARR_SIZE;i++)cout << A[i] << endl;
	cout << "\nOdd Count : " << count << endl;
}
```
### c
![](4-c.jpg)
```cpp
#include <iostream>

using namespace std;

int main(){

	const int ARR_SIZE = 20;
	float X[ARR_SIZE];

	float sum = 0;

	for(int i=0;i<ARR_SIZE;i++){
		cout << "Enter #"<<i+1<<": ";
		cin >> X[i];
		sum+=X[i];
	}

	cout << "Array :\n";
	for(int i=0;i<ARR_SIZE;i++)cout << X[i] << endl;
	cout << "\nSum : " << sum << endl;
	cout << "Avg : " << sum/ARR_SIZE0 << endl;
}
```

## Chapter 3 Answers
***
**Questions index:**     
[1](#1) . [2](#2) . [3](#3) . [4](#4) . [5](#5) . [6](#6) . [7](#7) . [8](#8) . [9](#9) . [10](#10) . [11](#11) . [12](#12) . [13](#13) . [14](#14) . [15](#15) . [16](#16) . [17](#17) . [18](#18) . [19](#19) . [20](#20) . [21](#21) . [22](#22) . [23](#23) . [24](#24) . [25](#25) . [26](#26) . [27](#27)
***
#### 1.
**Modify the program in Example 3.1 so that it prints a response only if n is divisible by d.**    
````cpp
int main()
int main() {
	int n, d;
	cout << "Enter two positive integers: ";
	cin >> n >> d;
	if (n%d == 0) cout << n << " is not divisible by " << d << endl;
}
````
#### 2.
**Modify the program in Example 3.1 so that it prints the minimum of four input integers**
````cpp
int main() {
	int n1,n2,n3,n4;
	cout << "Enter 4 integers: ";
	cin >> n1 >> n2 >> n3 >> n4;
	int min = n1;
	if (n2 < min) min = n2;
	if (n3 < min) min = n3;
	if (n4 < min) min = n4;
	cout << "Their minimum is " << min << endl;
}
````
#### 3.
#### 4.
#### 5.
#### 6.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int age;
	cout << "Enter your age:";
	cin >> age;
	if(age < 18){
		cout << "You are a child\n";
	}else if(age < 65){
		cout << "You are an adult\n";
	}else{
		cout << "You are a senior citizen\n";
	}
}
```
#### 7.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num1,num2;
	cout << "Enter first number:";
	cin >>  num1;
	cout << "Enter second number:";
	cin >> num2;

	if(num1%num2==0){
		cout << "multiple\n";
	}else{
		cout << "not\n";
	}
}
```
#### 8.
```cpp
#include <iostream>

using namespace std;

int main()
{
    cout << "Calculator !" << endl;

    int num1,num2;
    float result;
    char oprator;

    while (1){
        cout << "\n\n";
        cout << "X = ";
        cin >> num1 >> oprator >> num2;
        switch (oprator){
            case '+': result = num1 + num2; break;
            case '-': result = num1 - num2; break;
            case '*': result = num1 * num2; break;
            case '/': result = num1 / num2; break;
            case '%': result = num1 % num2; break;
            default: cout << "Unknown oprator '" << oprator << "'."; continue;
        }
        cout << "  = " << result;

    }

    return 0;
}
```
#### 9.
لعبة طوبة ورقة مقص
```cpp
#include<iostream>
using namespace std;

int main ()
{
	enum Move {ROCK,PAPER,SCISSORS};
	enum Result {WIN,LOSS,TIE};

	Move player1Move, player2Move;
	Result player1Result;
	int choice1,choice2;

	cout << "Choose your move.\n";
	cout << "1)Rock    2)Paper    3)Sossors\n\n";
	cout << "Player 1:";
	cin >> choice1;
	cout << "Player 2:";
	cin >> choice2;

	switch(choice1){
		case 1:
			player1Move = ROCK;
			break;
		case 2:
			player1Move = PAPER;
			break;
		case 3:
			player1Move = SCISSORS;
			break;
	}

	switch(choice2){
		case 1:
			player2Move = ROCK;
			break;
		case 2:
			player2Move = PAPER;
			break;
		case 3:
			player2Move = SCISSORS;
			break;
	}

	if(player1Move == player2Move){
		player1Result = TIE;
	}else{

		switch(player1Move){
			case ROCK:
				if(player2Move == SCISSORS)player1Result=WIN;
				else player1Result=LOSS;
				break;

			case PAPER:
				if(player2Move == ROCK)player1Result=WIN;
				else player1Result=LOSS;
				break;

			case SCISSORS:
				if(player2Move == PAPER)player1Result=WIN;
				else player1Result=LOSS;
				break;
		}
	}

	if(player1Result == TIE){
		cout << "\nResult: Tie !\n";
	}else if(player1Result == WIN){
		cout << "\nResult: Player 1 Wins\n";
	}else{
		cout << "\nResult: Player 2 Wins\n";
	}


}
```
#### 10.
#### 11.
#### 12.
```cpp
#include<iostream>
#include<cmath>
using namespace std;

int main ()
{
	//coefficients
	double a,b,c;
	//roots
	double x1,x2;

	cout << "ax^2 + bx + c = 0\n";
	cout << "a:";
	cin >> a;
	cout << "b:";
	cin >> b;
	cout << "c:";
	cin >> c;

	x1 = (-b + sqrt(b*b - 4*a*c))/2*a;
	x2 = (-b - sqrt(b*b - 4*a*c))/2*a;

	cout << "Root 1: " << x1 << endl;
	cout << "Root 2: " << x2 << endl;

}
```
#### 13.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int number,sum;
	cout << "Enter Number:";
	cin >> number;

	for(int i=1;i<=100000;i*=10){
		sum += (number/i)%10;
	}

	cout << "The sum of the digits is "<<sum<<endl;
}
```
#### 14.
#### 15.
```
0
0
0
```
#### 16.
```cpp
a) while(e)s;
b) while(true)s;e;
```
#### 17.
```cpp
int n = 15;
int i = 1;
while(i<=n){
	cout << i*i << " ";
	i++;
}
```
#### 18.
``1	1	3	9	5	9	7	7	``
#### 19.
```
1
End of program.
End of program.
3
End of program.
5
End of program.
End of program.
```
#### 20.
#### 22.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num,sum;
	cout << "Enter Number:";
	cin >> num;
	int i = 1;
	while(i<=num){
		sum+= i*i;
		i++;
	}
	cout << sum;
}
```
#### 21.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num,sum;
	cout << "Enter Number:";
	cin >> num;
	for(int i=1;i<=num;i++)sum+= i*i;
	cout << sum;
}
```
#### 23.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num,sum;
	cout << "Enter Number:";
	cin >> num;
	int i = 1;
	do{
		sum+= i*i;
		i++;
	}while(i<=num);
	cout << sum;
}
```
#### 24.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num1,num2;
	cout << "Enter number 1:";
	cin >> num1;
	cout << "Enter number 2:";
	cin >> num2;

	int result,remainder;
	result = num1/num2;
	remainder = num1%num2;

	cout << num1<<"/"<< num2 << " = "<< result << " + (" << remainder << "/"<<num2<<")\n";
}
```
#### 25.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num;
	cout << "Enter Your number:";
	cin >> num;
    int new_num = 0;
    while(num > 0)
    {
		new_num *=10;
		new_num += (num % 10);
        num /= 10;
    }
    cout << new_num << endl;
}
```
#### 26.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num = 8;
    double estimateRoot=num/2;
    for (int i = 1; i <= 1000; i++){
      estimateRoot=(estimateRoot+num/estimateRoot)/2;
    }
    cout << "square root of " << num << " is "<< estimateRoot << endl;
}
```
#### 27.
```cpp
#include<iostream>
using namespace std;

int main ()
{
	int num;
	cout << "Enter Your number:";
	cin >> num;

    int diff;
    int i=0;
    do{
		i++;
		diff = i*i - num;
	}while(diff<=0);

	cout << i-1;

}
```

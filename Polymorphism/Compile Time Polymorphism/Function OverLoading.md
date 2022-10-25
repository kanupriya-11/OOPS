# Function Overloading
In C++, two functions can have the same name if the number and/or type of arguments passed is different.

_***Overloaded functions may or may not have different return types but they must have different arguments.***_

### Some Examples of Function Overloading:-

1. Overloading Using Different Types of Parameter

```
// Program to compute absolute value
// Works for both int and float

#include <iostream>
using namespace std;

// function with float type parameter
float absolute(float var){
    if (var < 0.0)
        var = -var;
    return var;
}

// function with int type parameter
int absolute(int var) {
     if (var < 0)
         var = -var;
    return var;
}

int main() {
    
    // call function with int type parameter
    cout << "Absolute value of -5 = " << absolute(-5) << endl;

    // call function with float type parameter
    cout << "Absolute value of 5.5 = " << absolute(5.5f) << endl;
    return 0;
}


OUTPUT:-

Absolute value of -5 = 5
Absolute value of 5.5 = 5.5
```
<br>
<br>

2. Overloading Using Different Number of Parameters

```
#include <iostream>
using namespace std;

// function with 2 parameters
void display(int var1, double var2) {
    cout << "Integer number: " << var1;
    cout << " and double number: " << var2 << endl;
}

// function with double type single parameter
void display(double var) {
    cout << "Double number: " << var << endl;
}

// function with int type single parameter
void display(int var) {
    cout << "Integer number: " << var << endl;
}

int main() {

    int a = 5;
    double b = 5.5;

    // call function with int type parameter
    display(a);

    // call function with double type parameter
    display(b);

    // call function with 2 parameters
    display(a, b);

    return 0;
}


OUTPUT:-

Integer number: 5
Float number: 5.5
Integer number: 5 and double number: 5.5
```

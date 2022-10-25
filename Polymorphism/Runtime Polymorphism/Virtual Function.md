# Virtual Function

- Virtual : Anything which exists in appeareance but not there in reality.
- Virtual Function : a function which exists -is in the class but not in use.

### Why do we need Virtual Function?

We need virtual function to ensure that we call correct function using reference or pointer.

## 2 Cases:-

#### 1. With using "Virtual Function" :

```
#include <iostream>
using namespace std;

class Base
{
    public:
      virtual void msg()
      {
          cout<<"Base class function"<<endl;
      }
};

class derived : public Base
{
    public:
      void msg()
      {
          cout<<"Derived class function"<<endl;
      }  
};

int main()
{
    Base *ptr;
    ptr = new derived;
    ptr->msg();
    
    return 0;
}
OUTPUT:-

Derived class function
```

#### 2. Without using "Virtual Function" : 

```
#include <iostream>
using namespace std;

class Base
{
    public:
      void msg()
      {
          cout<<"Base class function"<<endl;
      }
};

class derived : public Base
{
    public:
      void msg()
      {
          cout<<"Derived class function"<<endl;
      }  
};

int main()
{
    Base *ptr;
    ptr = new derived;
    ptr->msg();
    
    return 0;
}

OUTPUT:-

Base class function
```

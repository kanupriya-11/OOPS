# Encapsulation

Wrapping up of Data members and Member functions together is called Encapsulation.

Eg:-

In C++, we can bundle data members and functions that operate together inside a single class. For example,

<pre>
class Rectangle {
  public:
    int length;
    int breadth;

    int getArea() {
      return length * breadth;
    }
};
</pre>
In the above program, the function getArea() calculates the area of a rectangle. To calculate the area, it needs length and breadth.

Hence, the data members (length and breadth) and the function getArea() are kept together in the Rectangle class.

## **Very Very IMPO:**

```Note:``` People often consider encapsulation as data hiding, but that's not entirely true.

Encapsulation refers to the bundling of related fields and methods together. This can be used to achieve data hiding. Encapsulation in itself is not data hiding.


## Why Encapsulation?

-In C++, encapsulation helps us keep related data and functions together, which makes our code cleaner and easy to read.

-It helps to control the modification of our data members.


## About Getter and Setter Functions:-

The getter and setter functions provide read-only or write-only access to our class members.

eg:-

Consider a situation where we want the length field in a class to be non-negative. Here we can make the length variable private and apply the logic inside the method setAge(). For example,

<pre>
class Rectangle {
  private:
    int age;

  public:
    void setLength(int len) {
      if (len >= 0)
        length = len;
    }
};
</pre>

The getter and setter functions provide read-only or write-only access to our class members. For example,

```
getLength()  // provides read-only access
setLength()  // provides write-only access
```


# Operator Overloading

In C++, we can change the way operators work for user-defined types like objects and structures. This is known as operator overloading.

### Syntax for C++ Operator Overloading

To overload an operator, we use a special operator function. We define the function inside the class or structure whose objects/variables we want the overloaded operator to work with.

```
class className {
    ... .. ...
    public
       returnType operator symbol (arguments) {
           ... .. ...
       } 
    ... .. ...
};
```

Here,

```returnType``` is the return type of the function. <br>
```operator``` is a keyword. <br>
```symbol``` is the operator we want to overload. Like: +, <, -, ++, etc. <br>
```arguments``` is the arguments passed to the function. 

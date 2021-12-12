# Ampersand {&} and const Report
## Usages of ampersand {&} operator:
### *Case 1:*
1. It is used as a condition --> code:: int main(){ if(a==5 && b==6) return a,b; }

### *Case 2:*
2. Use & to declare a reference to a type.
####Explanation..
When you use & in the left-hand side of a variable declaration, you're expecting a reference to the declared type. It can be used in any type of declarations (local variables, class members, method parameters).
####Code..
string mrSamberg("Andy");
string& theBoss = mrSamberg;

### *Case 3:*
3. Use & to get the address of a variable
####Explanation..
When you use & in the right-hand side of an expression, its meaning changes. In fact, it must be used in a variable declaration on the left-hand side, but it can also be used in assignments on the right-hand side.

It's also known as the "address-of operator" when used on the right-hand side of a variable. Not surprisingly if you put it in front of a variable, it'll return its address in the memory instead of the variable's value itself. It's useful for declaring pointers.
####Code..
string mrSamberg("Andy");
string* theBoss;

theBoss = &mrSamberg;
### *Case 4:*
4. Use & as a bitwise operator
####Explanation..
The bitwise AND is what it's called. It's an infix operator that takes two numbers as inputs and performs an AND on each of the inputs' bit pairs. Here's an illustration. 14 is represented as 1110 as a binary number and 42 can be written as 101010. As a result, 1110 (14) will be zero filed from the left, and the operation will proceed as follows.
####Code..
int data = 5 & 6;

## Usages of const keyword:
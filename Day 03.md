Anonymous function: 

The function without function name is anonymous function
mostly used while creaing methods
syntex:
() {
statements;
}

```void main() {
  (){
    print("ananymous function");
  } ();                                      "calling this near the function"
}```

output:
ananymous function

```void main() {
  (name){
    print(name);
  } ("inshira");
}```

output:
inshira

Operators and its types:
Arithmetic operators
```void main() {
  int a = 10, b = 20;
  
  int add = a + b;
  print(add);
  int sub = a - b;
  print(sub);
  int multi = a * b;
  print(multi);
  double div = a / b;
  print(div);
  int anotherdiv = a ~/ b;         "prints in integer of division operator ans before decimal"
  print(anotherdiv);
  int mod = a % b;
  print(mod);
}```

output:
30
-10
200
0.5
0
10

Assignments operators

```void main() {
  int a = 10;
  double b = 30;
  a += 10;
  print(a);
  a -= 5;
  print(a);
  a *= 2;
  print(a);
  a ~/= 2;
  print(a);
  b /= 2;
  print(a);
}```

output:

20
15
30
15
15

Relational "

```void main() {
  int a = 10;
  int b = 20;
  print(a>b);  
  print(a<b);  
  print(a>=b);  
  print(a<=b); 
  print(a==b);
  print(a!=b);  
}```

output
false
true
false
true
false
true

Incremen and Decrement operators
Postfix
```void main() {
  int a = 10;
  print(a++);
  print(a); 
}```

output:
10
11

prefix
```void main() {
  int a = 10;
  print(--a);  
}```

output:
9

Locical operators: used in conditions

&& - and
|| - or
! - not

Bitwise operators:
  used maily for who works in binarry num, ECE, iot students
  ```void main() {
  print(5&6);    and                  eg for how and work:    101 - 5
  print(5|6);    or                                           110  - 6
  print(5^6);    not                                          -----
  print(5<<1);   left shift                                   100 - 4
  print(5>>1);   right shift
}```                                  eg for how left shift   0101 - 5         it shift 1 time from 3rd digit to leftside
                                                              1010 - 2
output:
4
7
3
10
2


Typetest operators:

void main() {
  int a = 10;
  List b=[];
  print(a is int);
  print(a is double);
  print(a is! double);
  print(b is List);
}

output
true
true
false
true

Conditional operators:

```void main() {
  print(5>8 ? true:false);
  print(5>8 ? 5:8);
}```

output:
false
8


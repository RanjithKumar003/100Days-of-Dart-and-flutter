## Welcome to learn Dart and flutter

Introduction to Dart:

It is a client optimized program and to develop various apps in multiple platform
Developed by google
Use to develop mobile, desktop, server and web apps
It is ool and garbage collaction with c style syntax
Compiled to native code or js

Why we need dart ?

Used to build apps to cross platform
Not only UI and also web server applications
We can build web apps, mobile apps and desktop apps

Dart vs Js

Dart does not replace Js
But it substitute for Js.
Dart can also used for server side, so its a full stack.

Hello world program

```void main() {
  print("Hellow world");
}```

output:
Hello world

why main() ?
dart code does not execute without main function
it start compilation from main
outside function run through main function

Data types and iable:

6 types of data types are:
Set, num, string, list, boolean and map

Variables are storagers to store values

```void main() {
  num a = 3;
  num b = 2.4;
  print(a);
  print(b);
}```

outpu:
3
2.4

```void main() {
  int a = 3;
  int b = 2.4;
  double c = 2;         "it will take 2.0 indirectly"
  double d = 2.5;
  print(a);
  print(b);
  print(c);
  print(d);
}```


```void main() {
  String a = "Ranjith";
  bool isvalid = false;
  print(a);
  print(isvalid);
}```

output:
Ranjith
false

```void main() {
  num a =10;                 "insted of num u can try int and double"
  int b = -10;
  print(a.isNegative);
  print(b.isNegative);
  print(a.isOdd);
}```

output:
false
true
false

```void main() {
  num a = 10;
  num b = 80;
  double c = 3.7;
  double d = 22.45678;
  print(a.toString());
  print(b.toDouble());
  print(c.toInt());
  print(d.toStringAsFixed(2));
  print(e.length);
  print(e.isEmpty);
  print(e.toLowerCase);
  print(e.toUpperCase);
}```

output:
10
80
3
22.45
5
false
hello
HELLO

What is dynamic?
Dart is optionaly typed language
static run and gives output when all the code is typed, but dynamic is line by line
in static we should mention data types

``` void main() {
   var a = 7;
   dynamic s  = "ranjith"             "var or dynamic is dynamic data type"
   print(a is dynamic);
   print(s);
 }```
 
 output:
 true
 ranjith
 

 

Object orented programing:

Classes:
it is a blue print, it have variable and methods
dart is also object orented paradigm
we can create class useing class keyword

```class Person{
  String name = "ranjith";
  }

void main() {
  Person person = Person();
  print(person);
}``

output:
Instance of 'Person'

```class Person{
  String name = "ranjith";
  }

void main() {
  Person person = Person();
  print(person.name);
}``

output:
ranjith

```class Person{
  String name = "ranjith";
  void hello(){
    print("iam from class");
  }
  }

void main() {
  Person person = Person();
  print(person.name);
  person.hello();
}```

output:
ranjith
iam from class

constroctor:

````class Person{
  String name;
  Person({String name}){
    this.name = name;
  }
  void sayName(){
    print(this.name);
  }
}

void main() {
  Person ram = Person(name:"ram");
  print(person.name);
  ram.sayName();
}```

output:
ram

Nmaed constractor:

```class Person{
  String name;
  int age;
  Person({String name}){
    this.name = name;
  }
  Person.age({int age}){
    this.age = age;
  }
  void sayName(){
    print(this.name);
  }
}

void main() {
  Person ram = Person.age(21);
  print(ram.age);
}```

output:
21

```class Person{
  String firstname;
  String lastname;
  int age;
  bool isEmployed;
  Person({String fname, String lname, int age, bool isEmployed}){                 """instance variable"""
    this.firstname = fname;
    this.lastname = lname;
    this.age = age;
    this.isEmployed;
  }
}

void main() {
  Person ram = Person(fname:"ranjith",lname:"b",age: 21, isEmployed: false );
  print(ram.firstname);
  print(ram.lastname);
  print(ram.age);
  print(ram.isEmployed);
}```

output:
ranjith
b
21
null

```class Person{
  String firstname;
  String lastname;
  int age;
  bool isEmployed;
  Person({String fname, String lname, int age, bool isEmployed}){
    this.firstname = fname;
    this.lastname = lname;
    this.age = age;
    this.isEmployed;
  }
  void sayhello(String name){          """instance method"""
    print("hello " + name);
  }
}

void main() {
  Person ram = Person(fname:"ranjith",lname:"b",age: 21, isEmployed: false );
  print(ram.firstname);
  print(ram.lastname);
  print(ram.age);
  print(ram.isEmployed);
  ram.sayhello("krishna");
}```

output:
ranjith
b
21
null
hello krishna

getter:

```class Person{
  String firstname;
  String lastname;
  int age;
  
  String get fullname => this.firstname + this.lastname;

  Person({String fname, String lname, int age, bool isEmployed}){
    this.firstname = fname;
    this.lastname = lname;
    this.age = age;
  }
}

void main() {
  Person ram = Person(fname:"ranjith",lname:"kumar",age: 21, isEmployed: false );
  print(ram.fullname);
}```

output:
ranjithkumar

setter:
```class Person{
  String firstname;
  String lastname;
  int age;
  int birthyear;
  
  String get fullname => this.firstname + this.lastname;
  
  void set setBirthyear(int currentyear){
    this.birthyear = currentyear - this.age;
  }

  Person({String fname, String lname, int age, bool isEmployed}){
    this.firstname = fname;
    this.lastname = lname;
    this.age = age;
  }
}

void main() {
  Person ram = Person(fname:"ranjith",lname:"kumar",age: 21, isEmployed: false );
  print(ram.fullname);
  ram.setBirthyear = 2020;
  print(ram.birthyear);
}```

output:
ranjithkumar
1999

```class Parent{
  
  String parentname = "Parent";
  void parentmethod(){
    print("iam from parent");
  }
}
class Child extends Parent{
  
  String childname = "child";
  void childmethod(){
    print("iam from child");
  }
}

void main() {
  Child child = Child();
  print(child.parentname);
  child.parentmethod();
}```

output:
Parent
iam from parent

override:

```class Parent{
  
  String parentname = "Parent";
  void parentmethod(){
    print("iam from parent");
  }
}
class Child extends Parent{
  
  String childname = "child";
  @override
  void parentmethod(){
    print("iam from child");
  }
  void childmethod(){
    print("iam from child");
  }
}

void main() {
  Child child = Child();
  print(child.parentname);
  child.parentmethod();
}```

output:
Parent
iam from child

Enum - enumeration:
like genter form in website

```enum gender{
  Male,
  Female,
  Others
}

void main() {
  print(gender.value);
  print(gender.Female);

}```

output:
[gender.Male, gender.Female, gender.Others]
gender.Female

Mixins:
using methods from one class to another withot creating extends.

```class A{
  void aprint(){
     print("from a");
  }
}

class B with A{
  void bprint(){
    aprint();
    print("from b");
  }
}
void main() {
  B b = B();
  b.bprint();
}```

output:
from a
from b

static variabel and meethods:
accessing properties from class without creating instance, bu using static keyword

```class A{
  static String name = "inshira";
  static void hello() {
     print("hello");
  }
}

void main() {
  print(A.name);
  A.hello();
}```

output:
inshira
hello

library:
set of propeties, methods togeher call library

```import 'dart:math';
void main() {
  print(sqrt(16));
}```

output;
4

```import 'dart:math' as math;
void main() {
  print(math.pi);
  print(math.min(20,5));
  print(math.Random().nextInt(8));
}```

output:
3.141592653589793
5
1

## List, Set, map, and function

list:

 ```void main() {
   List mylist = [1,3,4.5,"hello"];
   List <int> list2 = [1,4,6];           "specific data type in list"
   print(mylist);
 }```
 
 output:
 1, 3, 4, 5, hello
 
  ```void main() {
   List mylist = [1,3,4.5,"hello"];
   mylist.add(3);
   List <int> list2 = [1,4,6];   
   print(mylist);
 }```
 
 output:
 1, 3, 4, 5, hello,3
 
 ``` void main() {
   List myAnotherList = List();
   print(myAnotherList);
   myAnotherList.add(1);
   print(myAnotherList);
 }```
 
 output:
 []
 [1]
 
 ```void main() {
   List mylist = [1,3,4.5,"hello"];
   mylist.removeAt(3);        
   print(mylist);
   mylist.removeLast();
   print(mylist);
 }```
 
 output:
 
 1,3,4,hello
 1,3,4
 
 
 ```void main() {
   List mylist = [1,3,4.5,"hello"];
   mylit[-1] = "ranjith"       
   print(mylist);
 }```
 
 output:
 1,3,4,5,ranjith
 
 Map or dictionary:
 ```void main() {
  Map mymap ={"name" : "ranjith"};        "in defult it is dynamic"
  print(mymap);
 }```
 
 output:
 
 {"name" : "ranjith"}
 
  ```void main() {
     Map <String.String> mymap ={"name" : "ranjith"};        "now the key and value are string"
     print(mymap);
    }```
 
  ```void main() {
     Map <String.String> mymap ={"name" : "ranjith"};        "now the key and value are string"
     print(mymap);
    }```

```void main() {
  Map <String.dynamic> mymap ={"name" : "ranjith", "age": 20};
  print(mymap);
  print(mymap.keys);
 }```
 
 output
 {name : ranjith, age: 20}
 {name, age}
 
 Set:
 it is unorderd
 all the elements must be unique
 
 ```void main() { 
  var persons = <String>{"John", "Doe", "Smith", "Alex"};
  print(persons);
  persons.remove("Doe");
  print(persons);
}```

output:
{John, Doe, Smith, Alex}

 ```void main() { 
  var persons = <String>{"John", "Doe", "Smith", "Alex", "Smith"};
  print(persons);
  persons.remove("Doe");
  print(persons);
}```

output:
{John, Doe, Smith, Alex}         "it ignore the repetation"

final keword:
once we decler a variable by using final keyword, we cant change the value after that 
eg; final int a = 10; "here after the 10 cant change "

```void main() {
  final name = "ranjith";
  print(name);
}```
output
ranjith

```void main() {
  final name = "ranjith";
  print(name);
  name = "inshira"
}```

output:
error

const:
```void main() {
  const pi = 3.14;
  print(pi);
  const = 4.4
}```

output:
error

const is same like as final, but cont is one time compile, final compile at the end

functions:
it cointins a Set of statements that are reuseable
when ever we need we can call and use

syntax:
returntype functionname{
statements;
}

main(){
  functionname();         A
 }

```void hello(){
  print("function");
}

void main() {
  hello();
}```

output:
function

```int add(){
  int a = 10;
  int b = 20;
  int c = a+b;
  return c;
}

void main() {
  int addition = add();
  print("addition");
}```

output:
30

parameters
  optional parameters
    named (by using name)
    positional (by using position)
    defult
  required parameters

optional parameter:
```void person(String name, int age){     "data types is not necesory, if we need we can add"
  print(name);
  print(age);
}

void main() {
  person("name: ranjith", age: 21);      "disadvantge in this valu will place if u give unorder"
}```

output
ranjith
21
```void person(String name, int age){     "data types is not necesory, if we need we can add"
  print(name);
  print(age);
}

void main() {
  person(21, "ranjith");      "if u want to give parameter correctly u need to go with named parameter"
} ```

output
21
ranjith


```void person(String name, int age, [isEmployed = false]){     
  print(name);
  print(age);
  print(isEmployed);
}

void main() {
  person("ranjith", 21, true);     "if the person change in parameter then only its true, otherwise it will defulty false"
} ```

output:
ranjith
21
true

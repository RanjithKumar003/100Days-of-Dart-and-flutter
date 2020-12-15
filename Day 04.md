#Controlflow and list of statements

to get input:
String name = stdin.readLineSync();   - string
var age = int.parse(stdin.readLineSync());  - int


it cointains looping and branching statements and also break and continue.

iF condition

```Syntax:
if (condition){
  statement;
}```

```void main() {
  int age = 20;
  if (age >= 18){
    print("you are an adult");
  }
}```

output:
you are an adult

if-else condition:
```Syntax:
if (condition){
  statement;
}
else{
  statement;
}```

```void main() {
  int age = 16;
  if (age >= 18){
    print("you are an adult");
  }
  else{
    print("not an adult");
  }
}```

output:
not an adult

else is condition:

```Syntax:
if (condition){
  statement;
}
else if (condition){
  statement;
}
else{
  statement;
}```


```void main() {
  int age = 13;
  if (age >= 1 && age < 11){
    print("babbies");
  }
  else if (age >= 11 && age < 18){
    print("teeanage");
  }
  else if (age >= 18 && age < 50){
    print("adult");
  }
  else{
    print("older");
  }
}```

output
teeanage


Loop:

commonly used in all thee loops are
initial condition
tent condition
increment dectement

forloop:

syntac
```for(in,tc,in/dec){
    statements;
    }```
    
 ```void main() {
  for(int i = 0; i == 10; i++){
    print(i);
  }
}```

output:
0
1
2
3
4
5
6
7
8
9
10

 ```void main() {
  for(int i = 0; i == 10; i++){
    print(i);
  }
}```

output:
0
2
4
6
8
10

```void main() {
  for(String i = "ranjith; i == 10; i++){
    print(i);
  }
}```

while loop:

syntax:
```ic;
  while (tc){
    statement;
    inc/dec;
  }```
  
  
```void main() {
  int i = 10;
  while (i>=1){
    print(i);
    i--;
  }
}```

output:
10
9
8
7
6
5
4
3
2
1

do-while:
syntex:
```in c
  do{
    statements:
    inc/dec;
  }
  while (tc);
}```

```void main() {
  int i = 0;
  do{
    print(i);
    i++;
  }
  while (i<=6);
}```

output:
0
1
2
3
4
5
6

Break and continue and used in loops.

Break:

```void main() {
  for(int i = 0; i == 10; i++){
    print(i);
    if (i == 6){
      break;
    }
  }
}```

output:
0
1
2
3
4
5

continue:

```void main() {
  for(int i = 0; i == 10; i++){
    print(i);
    if (i == 6){
      continue;
    }
    print(i);
  }
}```

output:
0
1
2
3
4
5
6
7
8
9
10

switch case:

syntax:
```switch (con){
    case (con) : statemwnt;```
```void main() {
  String sesson  = "rainy";
  
  switch (sesson){
    case "summmer" : print("hot");
      break;
    case "winter" : print("cool");
      break;
    case "rainy" : print("too chill");
      break;
    default : print("it is not a sesson");
  }
}```

output:
too chill

```void main() {
  String sesson  = "burgger";
  
  switch (sesson){
    case "summmer" : print("hot");
      break;
    case "winter" : print("cool");
      break;
    case "rainy" : print("too chill");
      break;
    default : print("it is not a sesson");
  }
}```

output:
it is not a sesson


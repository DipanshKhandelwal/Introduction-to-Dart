# Introduction to Dart

### Hello World
```Dart
void main() {
	print('Hello, World');
}
```

### Variables

#### String
```Dart
var name = 'My Name';
```

#### Integer
```Dart
var year = 1998;
```

#### Double
```Dart
var height = 5.8;
```

#### List
```Dart
var myList = ['Item1', 'Item2', 'Item3', 'Item4'];
```

#### Object
```Dart
var post = {
    'author': 'My Name',
    'date': '12/06/1998',
    'content': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
};
```

### Control Flow Statements

#### If Else
```Dart
if (num%2 == 0) {
    print('Even number');
} else {
    print('Odd number');
}
```

#### For Loop
```Dart
for (var str in myList) {
    print(str);
}
```

```Dart
for (int i = 0; i<10; i++) {
    print(i);
}
```

#### While Loop
```Dart
while (i < 10) {
    print(i++);
}
```

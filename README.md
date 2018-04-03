# Introduction to Dart

### Hello World
```Dart
void main() {
	print('Hello, World');
}
```

### Variables
The Dart language has special support for the following types:
* numbers
* strings
* booleans
* lists (also known as arrays)
* maps
* runes (for expressing Unicode characters in a string)
* symbols


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

### Functions
```Dart
int fibonacci(int n) {
	if (n == 0 || n == 1) {
		return n;
	}
	return fibonacci(n - 1) + fibonacci(n - 2);
}

var result = fibonacci(20);
```

```Dart
bool isEven(int num) => num%2==0;

var result = isEven(20);
```

### Comments
```Dart
// One line comment.

/* Multi line comment. */
```

### Imports
```Dart
// Importing core libraries
import 'dart:async';
import 'dart:math';

// Importing libraries from external packages
import 'package:test/test.dart';

// Importing files
import 'path/to/my_other_file.dart';
import '../lib/samples/myfile.dart';
```

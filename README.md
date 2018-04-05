# Introduction to Dart
An introduction to [Dart Programming Language](https://www.dartlang.org/).
Test your code here at [DartPad](https://dartpad.dartlang.org/).

<img src="Logo.png">

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

### Object Oriented Approach
```Dart
import 'dart:math';

abstract class Shape {
    List<double> sides;
    double perimeter;
  
    Shape(this.sides) {
        this.perimeter = this.sides.reduce((a, b) => a + b);
    }

    double area(); 
}

class Triangle extends Shape {
    Triangle(double a, double b, double c) : super([a,b,c]);

    double area() {
        double s = this.perimeter/2;
        return sqrt(s * (s - sides[0]) * (s - sides[1]) * (s - sides[2]));
    }
}

class Rectangle extends Shape {
    Rectangle(double a, double b) : super([a,b]);

    double area() {
        return sides[0]*sides[1];
    }
}

void main() {
    Triangle triangle = new Triangle(3.0, 4.0, 5.0);
    Rectangle rectangle = new Rectangle(4.0, 5.0);
    print('Area of triangle is ${triangle.area()}, its perimeter is ${triangle.perimeter}');
    print('Area of rectangle is ${rectangle.area()}, its perimeter is ${rectangle.perimeter}');
}
```

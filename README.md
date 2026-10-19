# Dart Programming Language — Basic to Advanced

A structured, hands-on roadmap for learning **Dart from beginner to advanced level**, with examples, exercises, and projects to prepare for Flutter development.

## About Dart

Dart is a programming language developed by Google. It is commonly used with Flutter to build Android, iOS, web, and desktop applications from a shared codebase.

This repository is organized as a learning path. Study each topic in order, write the examples yourself, and complete the exercises before moving forward.

## Learning Objectives

By completing this roadmap, you should be able to:

- Understand Dart syntax, variables, and data types.
- Write programs using conditions, loops, functions, and collections.
- Apply object-oriented programming concepts.
- Use null safety and handle errors.
- Work with asynchronous operations using `Future`, `async`, `await`, and `Stream`.
- Understand modern Dart features and write maintainable code.
- Build console-based projects and prepare for Flutter development.

## Prerequisites

- A computer with internet access.
- Basic familiarity with using a terminal or code editor.
- No previous programming experience is required.

## Setup

### Option 1: Run Dart online

Use [DartPad](https://dartpad.dev/) to write and run Dart code in your browser without installing anything.

### Option 2: Install Flutter (includes Dart)

1. Follow the [Flutter installation guide](https://docs.flutter.dev/get-started/install).
2. Install an editor such as Visual Studio Code or Android Studio.
3. Verify your setup:

   ```bash
   flutter doctor
   dart --version
   ```

4. Create a Dart console project:

   ```bash
   dart create -t console dart_basics
   cd dart_basics
   dart run
   ```

## Learning Roadmap

### Level 1 — Fundamentals

1. Introduction to Dart
2. Dart syntax and comments
3. `main()` function and `print()`
4. Variables: `var`, `final`, and `const`
5. Data types: `int`, `double`, `String`, `bool`, and `dynamic`
6. Type inference and type conversion
7. String interpolation and string methods
8. Operators: arithmetic, comparison, logical, assignment, and null-aware
9. User input in console applications
10. Basic debugging and reading errors

**Practice projects**
- Personal information printer
- Simple calculator
- Temperature converter

### Level 2 — Control Flow and Collections

1. `if`, `else if`, and `else`
2. `switch` statements and expressions
3. `for`, `while`, and `do-while` loops
4. `break` and `continue`
5. Lists and list methods
6. Sets and unique values
7. Maps and key-value pairs
8. Collection iteration: `forEach`, `map`, `where`, `any`, and `every`
9. Spread operators and collection `if`/`for`
10. Sorting, filtering, and searching collections

**Practice projects**
- Number guessing game
- Student marks calculator
- Contact list using a `Map`
- Shopping cart using a `List`

### Level 3 — Functions

1. Declaring and calling functions
2. Parameters and return types
3. Positional and named parameters
4. Optional parameters and default values
5. Arrow functions
6. Anonymous functions and closures
7. Scope and variable lifetime
8. Higher-order functions
9. Recursion
10. Function types and callbacks

**Practice projects**
- Calculator using functions
- Reusable grade calculator
- List filtering and sorting utility

### Level 4 — Object-Oriented Programming (OOP)

1. Classes and objects
2. Fields, methods, and properties
3. Constructors
4. Named and factory constructors
5. `this` keyword
6. Encapsulation and library privacy
7. Getters and setters
8. Inheritance and `super`
9. Method overriding
10. Abstract classes
11. Interfaces and `implements`
12. Mixins and `with`
13. Static members
14. Enums
15. Generics

**Practice projects**
- Student management system
- Bank account simulation
- Library management system
- Employee and payroll system

### Level 5 — Null Safety and Error Handling

1. Nullable and non-nullable types
2. Nullable types with `?`
3. Null assertion operator `!` and when to avoid it
4. Null-aware operators: `??`, `??=`, and `?.`
5. `late` variables
6. `try`, `catch`, and `finally`
7. Throwing exceptions
8. Custom exception classes
9. Validating input and handling invalid data

**Practice projects**
- Validated registration form in a console app
- Safe calculator with error handling
- Student records with missing optional values

### Level 6 — Asynchronous Programming

1. Synchronous vs asynchronous execution
2. `Future`
3. `async` and `await`
4. Error handling in asynchronous code
5. `Future.wait`
6. `Stream` and stream subscriptions
7. Stream transformations
8. Generators: `async*`, `yield`, and `yield*`
9. Timers and asynchronous workflows
10. Understanding concurrency and event-loop basics

**Practice projects**
- Simulated login service
- Fetch and process sample API data
- Live number stream
- Concurrent task runner

### Level 7 — Files, Packages, and JSON

1. Importing libraries
2. Core libraries such as `dart:math`, `dart:convert`, and `dart:io`
3. Creating and using packages
4. Understanding `pubspec.yaml`
5. Installing dependencies with `dart pub add`
6. Encoding and decoding JSON
7. Converting JSON to model classes
8. Reading and writing files in console apps
9. Environment configuration basics
10. Organizing code across files and libraries

**Practice projects**
- JSON-based student records
- Notes app using local files
- Command-line expense tracker

### Level 8 — Modern and Advanced Dart

1. Records
2. Patterns and pattern matching
3. Destructuring
4. Sealed classes
5. Extension methods
6. Extension types
7. Typedefs
8. Callable objects
9. Iterables and lazy evaluation
10. Custom operators where appropriate
11. Isolates and CPU-intensive work
12. Code organization and API design
13. Effective Dart style and linting

> Some language features depend on your Dart SDK version. Use the current stable SDK and consult the official Dart documentation for version-specific details.

### Level 9 — Testing and Code Quality

1. Writing unit tests with `package:test`
2. Assertions and test expectations
3. Testing success and failure cases
4. Test setup and teardown
5. Mocking and dependency boundaries
6. Static analysis with `dart analyze`
7. Formatting with `dart format`
8. Reading stack traces
9. Refactoring and clean code principles
10. Git and GitHub workflow

## Code Examples

### 1. Hello, World!

```dart
void main() {
  print('Hello, World!');
}
```

### 2. Variables and Types

```dart
void main() {
  String name = 'Joyal';
  int age = 25;
  double height = 1.75;
  bool isLearningDart = true;

  print('Name: $name');
  print('Age: $age');
  print('Height: $height');
  print('Learning Dart: $isLearningDart');
}
```

### 3. Conditions

```dart
void main() {
  int marks = 82;

  if (marks >= 90) {
    print('Grade A');
  } else if (marks >= 75) {
    print('Grade B');
  } else if (marks >= 50) {
    print('Grade C');
  } else {
    print('Needs improvement');
  }
}
```

### 4. Loops and Lists

```dart
void main() {
  final List<String> languages = ['Dart', 'Flutter', 'JavaScript'];

  for (final language in languages) {
    print(language);
  }
}
```

### 5. Functions

```dart
int add(int a, int b) {
  return a + b;
}

void main() {
  print(add(10, 20));
}
```

### 6. Classes and Objects

```dart
class Student {
  final String name;
  final int age;

  Student({
    required this.name,
    required this.age,
  });

  void introduce() {
    print('My name is $name and I am $age years old.');
  }
}

void main() {
  final student = Student(name: 'Joyal', age: 25);
  student.introduce();
}
```

### 7. Null Safety

```dart
void main() {
  String? nickname;

  nickname = 'Jay';

  print(nickname ?? 'No nickname provided');
}
```

### 8. Asynchronous Programming

```dart
Future<String> loadMessage() async {
  await Future.delayed(const Duration(seconds: 1));
  return 'Data loaded successfully';
}

Future<void> main() async {
  print('Loading...');

  final message = await loadMessage();
  print(message);
}
```

## Project Roadmap

Build these projects in sequence:

| Project | Level | Skills practiced |
|---|---|---|
| Personal profile printer | Beginner | Variables, strings, output |
| Calculator | Beginner | Operators, functions, conditions |
| Number guessing game | Beginner | Loops, conditions, input |
| Student grade manager | Beginner–Intermediate | Collections, functions |
| Bank account simulator | Intermediate | Classes, encapsulation |
| Library management system | Intermediate | OOP, collections, validation |
| Expense tracker | Intermediate | Files, JSON, models |
| API data client | Intermediate–Advanced | Futures, HTTP, JSON |
| CLI task manager | Advanced | Packages, architecture, testing |

## Suggested Study Schedule

A suggested 8-week plan for consistent daily practice:

| Week | Focus |
|---|---|
| 1 | Syntax, variables, types, operators |
| 2 | Conditions, loops, collections |
| 3 | Functions and problem solving |
| 4 | Classes and OOP |
| 5 | Null safety and exceptions |
| 6 | Async programming, files, JSON |
| 7 | Advanced language features and packages |
| 8 | Testing and a final console project |

Your progress will depend on your experience and study time. Spend more time coding than passively watching tutorials.

## Daily Practice Routine

- **20% — Learn:** Read documentation or study a topic.
- **60% — Code:** Write examples and solve exercises.
- **20% — Review:** Debug, revise notes, and commit progress to Git.

## Recommended Resources

- [Dart official learning page](https://dart.dev/learn)
- [Dart language documentation](https://dart.dev/language)
- [Dart API reference](https://api.dart.dev/)
- [DartPad online editor](https://dartpad.dev/)
- [Effective Dart style guide](https://dart.dev/effective-dart)
- [Dart packages](https://pub.dev/)
- [Flutter documentation](https://docs.flutter.dev/)

## Completion Checklist

- [ ] I can write a Dart program independently.
- [ ] I understand variables, data types, and operators.
- [ ] I can use conditions, loops, and collections.
- [ ] I can write reusable functions.
- [ ] I understand classes, constructors, inheritance, and interfaces.
- [ ] I can use null safety and handle exceptions.
- [ ] I understand `Future`, `async`, `await`, and `Stream`.
- [ ] I can work with JSON and files.
- [ ] I can organize code into multiple files and packages.
- [ ] I can write and run tests.
- [ ] I have completed at least three console projects.
- [ ] I am ready to start learning Flutter widgets and app development.

## Next Step: Learn Flutter

After completing the Dart fundamentals and building a few console projects, continue with:

1. Flutter installation and project structure
2. Widgets and layouts
3. Navigation and forms
4. State management
5. REST API integration
6. Local storage and databases
7. Testing and deployment

---

**Keep practicing:** Write code every day, experiment with examples, and commit your progress to GitHub.

**Repository:** `Dart-Programming-Language`  
**Language:** Dart  
**Goal:** Beginner to Advanced Dart Programming
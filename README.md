# Flutter Interview Questions & Answers

Flutter is Google's easy User Interface toolkit for building beautiful, natively compiled applications for android, ios, web, and desktop from a single codebase.

## Getting Started

### How many types of widgets are there in Flutter?

There are two types of widgets:
* StatelessWidget : A widget that does not require mutable state.
* StatefulWidget: A widget that has mutable state.



## When to use main Axis Alignment and cross Axis Alignment?

`````
For Row:
mainAxisAlignment = Horizontal Axis
crossAxisAlignment = Vertical Axis

For Column:
mainAxisAlignment = Vertical Axis
crossAxisAlignment = Horizontal Axis
`````

## What is a null-aware operator, and how do we use it?
There are two null-aware operators — the first one is ??, and the second is ??=.
`````
Example: int x; x ??= 1, var x = y ?? 2
`````

## What’s a ‘Future’ in Dart?
It’s used for asynchronous programming. A Future represents a potential value (or error) that’ll be available at some time in the future.
Receivers of a Future can register callbacks that handle the value or error once it’s available.

## How can we parse JSON?
Dart provides this natively, and it’s available within the [dart:convert library](https://api.dart.dev/stable/2.7.2/dart-convert/dart-convert-library.html). There are jsonDecode and jsonEncode methods available.

## What’s the lifecycle of a ‘StatefulWidget’?
* createState() — a method in a StatefulWidget that’s called immediately and should return a State object for the widget
* initState() — the first method called in the State object after the widget is created
* didChangeDependencies() — called immediately after initState() the first time the widget is built
* build() — very similar to the one from the StatelessWidget. It’s called right after didChangeDependencies(). It’s called every single time the UI needs to render and returns a widget’s tree.
* didUpdateWidget() — it’s called when the parent widget changes and needs to redraw its UI
* deactivate() — called before dispose(), when this object is removed from the tree
* dispose() — called when deallocating the whole widget and its state

## What’s a pubspec.yml file?
It’s a file where you can provide all the dependencies (optional and required — e.g., plugins, Dart version, font, images) of your Flutter project. It’s also a place where you configure the project’s name and description.

## What’s a hot reload and a hot restart? What’s the difference?
The hot-reload feature allows you to quickly reload the code on a running app. It takes less time than hot restart, as the hot restart destroys and recreates all states in the app as well (and the whole widget tree is completely rebuilt).

## For More

Please visit interview questions
* [flutter interview questions](https://www.interviewquestions.app/flutter-interview-questions-answers-2021/)

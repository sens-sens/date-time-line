<!-- 
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages). 

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages). 
-->

A flutter package that can be used to import scrollable datetime timeline.

## Features

supports Web, Android  
can change Color according to your UI

![image](images/image.png)



## Getting started

To use this package add it to the pubspec.yaml and run 'flutter pub get'  
Now, you can import 'DateTimeLine()' widget and use it.

## Usage

Below is an example code for using this.
```dart
import 'package:date_time_line/date_time_line.dart';
```

```dart
DateTimeLine(
            width: MediaQuery.of(context).size.width,
            color: Colors.lightGreen,
            hintText: "10 task today",
            onSelected: (value) {
              setState(() {
                date = value;
              });
            },
          ),
```
The 'date' variable can be used to get the selected date.  
The 'hintText' value is shown below the month and year.
## Additional information
Currently i have tested it only on Android and Web. Soon i'll try to implement this on Windows, IOS ...

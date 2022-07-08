# C++ FString
**A quick C++ formatting library**

I was working on a logging library, and needed some way to format strings quickly, simple and clean, so I wrote this library.

This library is not the best in general, but for my project needs it is the fastest and the best

## Features
- **Easy**  include and just call `fstring()`
- **Fast**  Just a simple code to extract and modify the string
- **Light** No lots of code, just one class with only one function to call
- **CrossPlatform** It doesn't use any third party libraries, so it should work anywhere

## Syntax
```cpp
// parameters
fstring("{}, {}", "Hello","World"); // "Hello, World"

// padding
fstring("%5Hello%5World%5"); // "     Hello     World     "

// smart padding, divide string to section, final padding = padding - length of section
fstring("%.10Hello.%%.10World.%"); // "Hello     World     "

// result
fstring(..).get(); // return to &string
```

## Target
- Provides an easy, fast and clean way to format strings

- Providing the best performance for millions of times use

## Test Info
- **OS**: Ubuntu 22.04 LTS / 64-bit
- **Processor**: Intel® Core™ i7-6500U CPU @ 2.50GHz × 4
- **Compiler**: g++ 12
- **Flags**: -O3

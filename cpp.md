# C++
## Resources
- [cppreference.com](https://en.cppreference.com/w/)
- [learncpp.com](https://www.learncpp.com/)
- A Tour of C++ (2nd edition)
- Effective C++
- Effective Modern C++
- [Game Programming Patterns](http://gameprogrammingpatterns.com/contents.html)

## Basic Program
## Building with Makefiles
## Building with CMake

## I/O
```
// reading an integer from stdin
int n;
std::cin >> n;
```
- https://www.learncpp.com/cpp-tutorial/stdcin-and-handling-invalid-input/
  - `std::cin` may fail and initialize with:
    - 0, from invalid input
    - nothing (keeps initial value), from being in failure mode
    - closest in-range value, from overflow
  - `std::cin` will read until invalid input. To ignore rest of line:
```
std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
```
- error checking [`basic_istream`](https://en.cppreference.com/w/cpp/io/basic_istream): `good()`, `bad()`, `fail()`, `eof()`, `operator bool()` (`!fail()`)
- https://en.cppreference.com/w/cpp/io
- [`<iostream>`](https://en.cppreference.com/w/cpp/header/iostream)
- [`std::getline`](https://en.cppreference.com/w/cpp/string/basic_string/getline)
- [`std::stoi`](https://en.cppreference.com/w/cpp/string/basic_string/stol)

## Initialization
- [cppreference - Initialization](https://en.cppreference.com/w/cpp/language/initialization)
- [abseil / Tip of the Week #88: Initialization: =, (), and {}](https://abseil.io/tips/88)

## Error Handling
- https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-errors
- https://docs.microsoft.com/en-us/cpp/cpp/errors-and-exception-handling-modern-cpp?view=msvc-170
- https://www.cppstories.com/2018/05/errors-and-optional/
- error handling styles:
  - error code (C style)
  - `std::optional`
  - `std::variant`
  - `try`, `catch`, `throw`, `std::exception`
  - coming soon? `std::expected`
- [Back to Basics: Algebraic Data Types - Arthur O'Dwyer - CppCon 2020](https://youtu.be/OJzmWqCCZaM)
  - pair, tuple, optional, variant (runtime: 1:10:14)

## Differences from C
This section describes how the semantics of C style or C compatible code changes when compiled as C++.  
- [Compatibility of C and C++](https://en.wikipedia.org/wiki/Compatibility_of_C_and_C%2B%2B) on wikipedia.

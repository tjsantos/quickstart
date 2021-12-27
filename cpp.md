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

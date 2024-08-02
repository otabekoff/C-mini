# `C++ mini` Code Styling Guide

Welcome to the C++ Code Styling Guide for the Mini Projects Collection. Following a consistent style improves readability and maintainability of the code. Please adhere to the following guidelines when contributing to this repository.

## General Guidelines

- **Indentation**: Use 4 spaces for indentation. Do not use tabs.
- **Line Length**: Limit lines to 80 characters.
- **Braces**: Place braces on the same line as the statement they are associated with.
    
    ```cpp
    // Good
    if (condition)
    {
        // code
    }
    
    // Bad
    if (condition) {
        // code
    }
    ```
    
- **Comments**: Use comments to explain non-obvious parts of the code. Avoid redundant comments.
    
    ```cpp
    // Good
    // Calculate the area of a circle
    double area = M_PI * radius * radius;
    
    // Bad
    // This is a circle area calculation
    double area = M_PI * radius * radius;
    ```
    

## Naming Conventions

- **Variables**: Use `camelCase` for variable names.
    
    ```cpp
    int numberOfItems;
    double totalPrice;
    ```
    
- **Functions**: Use `camelCase` for function names.
    
    ```cpp
    void calculateTotalPrice();
    int findMaxValue(int a, int b);
    ```
    
- **Constants**: Use `UPPER_SNAKE_CASE` for constants and macros.
    
    ```cpp
    const int MAX_BUFFER_SIZE = 1024;
    ```
    
- **Classes**: Use `PascalCase` for class names.
    
    ```cpp
    class ShoppingCart;
    class InventoryManager;
    ```
    
- **Other cases:** They shouldn’t be used. But if it needs to be used so, then it is allowed to avoid conflicts.

## Code Organization

- **Include Guards**: Use include guards or `#pragma once` to prevent multiple inclusions.
    
    ```cpp
    #ifndef SHOPPING_CART_H
    #define SHOPPING_CART_H
    
    // class definition
    
    #endif // SHOPPING_CART_H
    ```
    
- **Namespaces**: Use namespaces to avoid name conflicts and organize code logically.
    
    ```cpp
    namespace project {
        class ShoppingCart {
            // class members
        };
    }
    ```
    
- **Header Files**: Use header files (`.h` or `.hpp`) for declarations and source files (`.cpp`) for definitions.

## Error Handling

- **Exceptions**: Use exception handling for error reporting and recovery.
    
    ```cpp
    try {
        // code that may throw exceptions
    } catch (const std::exception& e) {
        std::cerr << "Error: " << e.what() << std::endl;
    }
    ```
    
- **Error Codes**: If using error codes, define them clearly and use them consistently.
    
    ```cpp
    enum ErrorCode {
        SUCCESS = 0,
        ERROR_FILE_NOT_FOUND,
        ERROR_INVALID_INPUT
    };
    ```
    

## Code Formatting Tools

- **ClangFormat**: Use ClangFormat for automated code formatting. A configuration file (`.clang-format`) is provided in the repository.

## Example

Here’s a sample of properly styled C++ code:

```cpp
#include <iostream>
#include <cmath>namespace mini_projects {

class Circle {
    public:
        Circle(double radius) : radius(radius) {}
        double getArea() const;
    private:
        double radius;
    };

    double Circle::getArea() const {
        return M_PI * radius * radius;
    }

} // namespace mini_projects

int main() {
    mini_projects::Circle circle(5.0);
    std::cout << "Area: " << circle.getArea() << std::endl;
    return 0;
}
```

By adhering to these guidelines, we ensure that the code is clean, readable, and maintainable. Thank you for contributing to the Mini Projects Collection!

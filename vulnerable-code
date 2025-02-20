#include <iostream>
#include <cstring>
#include <memory>

// Vulnerability 1: Buffer Overflow
void buffer_overflow_example() {
    char buffer[10];
    std::cout << "Enter a string: ";
    std::cin >> buffer; // No bounds checking, can overflow buffer
    std::cout << "You entered: " << buffer << std::endl;
}

// Vulnerability 2: Null Pointer Dereference
void null_pointer_dereference_example() {
    int* ptr = nullptr;
    *ptr = 10; // Dereferencing a null pointer
}

// Vulnerability 3: Use-After-Free
void use_after_free_example() {
    int* ptr = new int(42);
    delete ptr; // Memory is freed
    *ptr = 100; // Using memory after it has been freed
}

// Vulnerability 4: Integer Overflow
void integer_overflow_example() {
    int max_int = 2147483647; // Maximum value for a 32-bit signed integer
    int result = max_int + 1; // Integer overflow
    std::cout << "Result of overflow: " << result << std::endl;
}

// Vulnerability 5: Uninitialized Variable
void uninitialized_variable_example() {
    int x;
    std::cout << "Uninitialized variable: " << x << std::endl; // Using uninitialized variable
}

// Vulnerability 6: Division by Zero
void division_by_zero_example() {
    int numerator = 10;
    int denominator = 0;
    int result = numerator / denominator; // Division by zero
    std::cout << "Result of division: " << result << std::endl;
}

// Vulnerability 7: Memory Leak
void memory_leak_example() {
    int* ptr = new int(100);
    // Forgot to delete ptr, causing a memory leak
}

int main() {
    std::cout << "Running vulnerable code examples..." << std::endl;

    // Uncomment to test specific vulnerabilities
    // buffer_overflow_example();
    // null_pointer_dereference_example();
    // use_after_free_example();
    // integer_overflow_example();
    // uninitialized_variable_example();
    // division_by_zero_example();
    // memory_leak_example();

    std::cout << "Finished running examples." << std::endl;
    return 0;
}

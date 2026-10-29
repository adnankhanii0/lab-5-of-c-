# lab-5-of-c-
C++, lab array , traversal, maximum, minimum values

# Arrays and Bubble Sort in C++

## 📌 Overview
This project covers arrays, array indexing, array traversal, 1D and 2D arrays, loops, and the Bubble Sort algorithm using C++.

## 🎯 Objectives
- Understand arrays in C++.
- Learn the difference between 1D and 2D arrays.
- Understand array indexing and traversal.
- Implement Bubble Sort.
- Learn the time complexity of sorting algorithms.

## 📚 Topics Covered

### 1. What is an Array?
An array is a collection of elements of the same data type stored under one name.

Example:
```cpp
int marks[5] = {70, 80, 65, 90, 75};
```

### 2. Types of Arrays

**1D Array:** Stores elements in a single list.
```cpp
int a[4] = {10, 20, 30, 40};
```

**2D Array:** Stores elements in rows and columns.
```cpp
int b[2][3] = {
    {10, 20, 30},
    {40, 50, 60}
};
```

### 3. Array Indexing
Array indexing is used to access elements by their position. In C++, indexing starts from `0`.

```cpp
int a[3] = {10, 20, 30};
cout << a[0]; // Output: 10
```

### 4. Array Traversal
Array traversal means visiting each element of an array, usually with a loop.

```cpp
for (int i = 0; i < 3; i++) {
    cout << a[i] << " ";
}
```

### 5. Bubble Sort
Bubble Sort compares adjacent elements and swaps them when they are in the wrong order.

Example:

Before sorting: `5, 3, 8, 1`

After sorting: `1, 3, 5, 8`

### 6. Why Use Arrays?
- Store multiple values under one name.
- Organize similar data.
- Access elements using indexes.
- Process data efficiently with loops.
- Perform searching and sorting operations.

### 7. Bubble Sort Time Complexity
- Best Case: `O(n)` with an optimized implementation.
- Average Case: `O(n²)`.
- Worst Case: `O(n²)`.

### 8. Array vs Variable
- **Variable:** Stores one value, such as `int x = 10;`.
- **Array:** Stores multiple values of the same data type.

### 9. Declaring a 2D Array
Syntax:
```cpp
data_type array_name[rows][columns];
```

Example:
```cpp
int marks[2][3];
```

### 10. Importance of Loops
Loops help us display, input, search, and process array elements without writing repetitive statements.

## 💻 Complete Bubble Sort Program

```cpp
#include <iostream>
using namespace std;

int main() {
    int a[] = {5, 3, 8, 1};
    int n = 4;

    for (int i = 0; i < n - 1; i++) {
        for (int j = 0; j < n - 1 - i; j++) {
            if (a[j] > a[j + 1]) {
                int temp = a[j];
                a[j] = a[j + 1];
                a[j + 1] = temp;
            }
        }
    }

    cout << "Sorted array: ";
    for (int i = 0; i < n; i++) {
        cout << a[i] << " ";
    }

    return 0;
}
```

### Output
```text
Sorted array: 1 3 5 8
```

## 🛠️ Requirements
- C++ compiler (G++, MinGW, or another compatible compiler)
- Visual Studio Code or any C++ IDE

## ▶️ How to Run
1. Save the program as `main.cpp`.
2. Open the terminal in the project folder.
3. Compile the program:

   ```bash
   g++ main.cpp -o main
   ```

4. Run the program:

   **Windows:**
   ```bash
   .\main.exe
   ```

   **Linux/macOS:**
   ```bash
   ./main
   ```

## 👨‍🎓 Learning Outcome
After completing this lab, students should understand arrays, loops, array traversal, and the implementation of Bubble Sort in C++.

## 📄 License
This project is intended for educational and learning purposes.


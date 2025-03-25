# C++ Style Guide

This style guide outlines the conventions used in this C++ project to maintain consistency and readability across the codebase.

---

## File Naming

- **Source files**: Use `.cc` for C++ source files.
- **Header files**: Use `.h` for C++ header files.

---

## Naming Conventions

- **Functions and variables**: Use `snake_case` (e.g., `calculate_sum`, `total_count`).
- **Structs and classes**: Use `PascalCase` (e.g., `MyClass`, `DataStructure`).
- **Constants**: Prefix with `k_` and use `snake_case` (e.g., `k_max_size`, `k_default_value`).
- **Member variables**: Use `snake_case_` suffix (e.g., `health_`, `position_x_`).
- **Namespaces**: Use `snake_case` (e.g., `project_namespace`).
- **Macros**: Use `UPPER_CASE` (e.g., `MAX_VALUE`, `DEBUG_MODE`).

---

## Header Files

- **Include guards**: Use `#ifndef FILE_NAME_H_`, `#define FILE_NAME_H_`, and `#endif`.
- **`#pragma once`**: Prefer `#pragma once` for simplicity.
- **Include order**:
  1. Own header file.
  2. System headers (e.g., `<iostream>`, `<vector>`).
  3. Third-party libraries (e.g., `<emscripten/html5.h>`).

---

## Comments

- **Single-line comments**: Use `//` for single-line comments.
- **Multi-line comments**: Use `/** ... */` for documentation or multi-line comments.

---

## Best Practices

- **Null pointers**: Prefer `nullptr` over `NULL`.
- **Explicit constructors**: Use `explicit` for single-argument constructors to avoid implicit conversions.
- **Smart pointers**: Avoid raw pointers; prefer `std::unique_ptr` or `std::shared_ptr` for memory management.
- **Use `const` for references**: When passing parameters by reference that are not modified, use `const` to ensure immutability (e.g., `const MyType& param`).
- **Use `constexpr` when possible**: Prefer `constexpr` for compile-time constants instead of `#define` or `const`.
- **Avoid magic numbers**: Define meaningful constants instead of using raw numeric values.
- **Minimize use of global variables**: Prefer encapsulation within classes or namespaces.

---

By following these guidelines, we can ensure clean, consistent, and maintainable code throughout the project.


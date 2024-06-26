# Java Conventions and Clean-Code Guides

This document outlines the conventions and clean code guidelines for the Loverary project. Following these guidelines ensures consistency, readability, and maintainability across the codebase.

## Table of Contents

1. [Naming Conventions](#naming-conventions)
2. [Code Formatting](#code-formatting)
3. [Commenting and Documentation](#commenting-and-documentation)
4. [Code Structure](#code-structure)
5. [Best Practices](#best-practices)
6. [Error Handling](#error-handling)
7. [Version Control](#version-control)

## Naming Conventions

### Classes and Interfaces

- **Class names** should be nouns, in mixed case with the first letter of each internal word capitalized.
  ```java
  public class LibraryManagementSystem { }
  ```

- **Interface names** should be adjectives, in mixed case with the first letter of each internal word capitalized.
  ```java
  public interface Borrowable { }
  ```

### Methods

- **Method names** should be verbs, in mixed case with the first letter lowercase and the first letter of each internal word capitalized.
  ```java
  public void borrowBook() { }
  ```

### Variables

- **Variable names** should be in mixed case with a lowercase first letter. Internal words should start with uppercase letters.
  ```java
  int bookCount;
  String userName;
  ```

- **Constants** should be all uppercase with words separated by underscores.
  ```java
  public static final int MAX_BOOKS_ALLOWED = 10;
  ```

### Packages

- **Package names** should be all lowercase, with consecutive words simply concatenated together.
  ```java
  package com.example.loverary;
  ```

## Code Formatting

### Indentation

- Use **4 spaces/1 tab** for indentation. 

### Line Length

- Limit lines to a maximum of **100 characters**.

### Braces

- **Braces** should be used for all control structures (if, else, for, while, etc.) and placed on the same line.
  ```java
  if (condition) {
      // code
  } else {
      // code
  }
  ```

### Spacing

- Use a **single space** before and after operators.
  ```java
  int sum = a + b;
  ```

- Do not add spaces between the method name and the parenthesis.
  ```java
  public void calculateSum(int a, int b) { }
  ```

## Commenting and Documentation

### Javadoc

- Use **Javadoc** for all public classes and methods.
  ```java
  /**
   * Represents a book in the library.
   */
  public class Book {
      /**
       * The title of the book.
       */
      private String title;
      
      /**
       * Gets the title of the book.
       *
       * @return the title of the book
       */
      public String getTitle() {
          return title;
      }
  }
  ```

### Inline Comments

- Use inline comments sparingly and only when the code is not self-explanatory.
  ```java
  // Initialize the book list
  List<Book> books = new ArrayList<>();
  ```

### Block Comments

- Use block comments to describe higher-level abstractions or complex code blocks.
  ```java
  /*
   * This method processes the list of books and updates the inventory.
   * It performs the following steps:
   * 1. Checks the availability of each book.
   * 2. Updates the inventory status.
   * 3. Sends notification if the book is not available.
   */
  ```

## Code Structure

### Organizing Code

- Group related methods together.
- Order methods by their importance and visibility: public, protected, private.

### Class Structure

1. Class variables (fields)
2. Constructors
3. Public methods
4. Protected methods
5. Private methods

### Avoid Long Methods

- Break down long methods into smaller, more manageable ones.

## Best Practices

### DRY (Don't Repeat Yourself)

- Avoid code duplication by abstracting common logic into methods or classes.

### KISS (Keep It Simple, Stupid)

- Write simple and straightforward code. Avoid unnecessary complexity.

### YAGNI (You Aren't Gonna Need It)

- Do not add functionality until it is necessary.

### Single Responsibility Principle

- A class should have only one reason to change. Each class should have a single responsibility.

### Avoid Magic Numbers

- Replace magic numbers with named constants.

### Encapsulation

- Use private fields and provide public getter/setter methods.



## Error Handling

### Exceptions

- Use exceptions for error handling, not for control flow.
- Catch specific exceptions instead of generic ones.
  ```java
  try {
      // code
  } catch (IOException e) {
      // handle exception
  }
  ```



## Version Control

### Branching Strategy

- Use `main` for production-ready code.
- Use `development` for ongoing development.
- Create feature branches from `development` and merge back into `development` when complete.

### Commit Messages

- Write clear, concise commit messages.
- Follow the format:
  ```plaintext
  type(scope): subject

  body
  ```

### Pull Requests

- Ensure your code is reviewed by at least one other team member.
- Provide a clear description of the changes.

By adhering to these conventions and guidelines, we can maintain a high standard of code quality and ensure our project remains clean, readable, and maintainable. Don't turn this repo into a garbage for your raggity code!
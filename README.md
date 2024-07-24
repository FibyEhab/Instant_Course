# Task 1
---
1. **What are the types of programming languages?**
2. **Pogramming language that support and not support automatic Garbage Collection.**
3. **The 13 principles of clean code.**
4. **How to implement `do while` in python?**
5. **Comparison between `for` and `while` in python.**
6. **Equivalent of `pass` in Java and C++**
7. **How to Write Directly in the Middle of a File?**
---
## Answers:

### 1. What are the types of programming languages?
#### 1. Low-Level Languages and High-Level Languages ####
##### Low-Level Languages:
- Machine Language: Consists of binary code that is directly executed by the computer's CPU.
- Assembly Language: Uses mnemonic codes to represent machine-level instructions.

#### High-Level Languages: ####
- Closer to human languages, making them easier to read and write. Examples: Python, Java.

#### 2. Compiled Languages, Interpreted Languages and Hybrid Languages ####
##### Compiled Languages: #####
- Translated into machine code by a compiler before execution. Example: C, C++, Rust.

##### Interpreted Languages: #####
- Executed line-by-line by an interpreter. Example: Python, Ruby, JavaScript.

##### Hybrid Languages: #####
- Use both compilation and interpretation. Example: Java (compiled to bytecode, interpreted by JVM).

#### 3. General-Purpose Languages and Domain-Specific Languages (DSLs) ####
##### General-Purpose Languages: #####
- Used for a wide variety of applications. Example: Python, C++, Java.

#####  Domain-Specific Languages (DSLs): #####
- Specialized for a specific application domain. Example:

   SQL (database queries), HTML (web pages), MATLAB (mathematical computing).

#### 4. Dynamic Languages and Static Languages ####
##### Dynamic Languages: #####
-  Type checking at runtime, more flexible, easier to write and modify, prone to runtime errors.

##### Static Languages: #####
- Type checking at compile-time, more robust and performant, but can be more verbose and less flexible.

#### 5. Programming Languages and Scripting Languages ####
##### Programming Languages: #####
- Generally compiled, used for creating standalone applications, offer high performance and static typing. Examples include C++ and Java.

##### Scripting Languages: #####
- Typically interpreted, used for automating tasks and adding functionality to existing applications, offer flexibility and easy of use.
- Examples include Python and JavaScript.

#### 6.Open Source Software and Closed Source Software ####
##### Open Source Software: #####
- Promotes collaboration and transparency, allowing anyone to use, modify, and distribute the software.
- Examples include Linux, Apache HTTP Server, and Mozilla Firefox.

##### Closed Source Software: #####
 - Maintains exclusive control over the software's source code, with usage governed by licensing agreements.
 - Examples include Microsoft Windows, Adobe Photoshop, and Microsoft Office.

#### 7.Supporting OOP and Not Supporting OOP ####
##### Supporting OOP: #####
- Include Java, Python, C++, and C#, which offer features like classes, inheritance, polymorphism, and encapsulation.
- These languages provide robust mechanisms for organizing and managing code.

##### Not Supporting OOP: #####
- Include C, Assembly Language, and Fortran.
- These languages follow different paradigms, such as procedural or functional programming,

   and may lack OOP features but can be simpler or more efficient for specific use cases.

### 3. The 13 principles of clean code.
**1. Meaningful Names:**
- Use descriptive and unambiguous names.
- Names should reveal the intent of the variable, function, or class.

**2. Single Responsibility Principle (SRP):**
- Each class or function should have one purpose or responsibility.
- This makes the code easier to understand and modify.

**3. Small Functions:**
- Functions should be small and do one thing only.
- They should be short enough to fit on one screen.
  
**4. Code Should Be Readable:**
- Write code that is easy to read and understand.
- Use proper indentation, spacing, and clear comments.
  
**5. Avoid Duplicate Code (DRY - Don't Repeat Yourself):**
- Avoid copying and pasting code.
- Reuse code through functions, classes, or modules.

**6. Expressive Code:**
- Code should clearly convey its intent.
- Use clear and descriptive variable and method names.
  
**7. Proper Error Handling:**
- Handle errors gracefully and predictably.
- Avoid using exceptions for normal flow control.
  
**8. Use of Comments:**
- Comment on why something is done, not what is done.
- The code itself should be self-explanatory.

**9. Consistent Code Formatting:**
- Follow consistent coding standards and style.
- Proper formatting improves readability and maintainability.
  
**10. Dependency Management:**
- Depend on abstractions rather than concrete implementations.
- Use dependency injection to manage dependencies.
  
**11. Testing:**
- Write automated tests to verify code functionality.
- Tests act as documentation for what the code is supposed to do.

**12. Avoid Side Effects:**
- Functions should not have hidden side effects.
- Ensure that state changes are predictable and clear.

**13. Code Simplicity:**
- Keep the code as simple as possible.
- Avoid unnecessary complexity; prefer straightforward solutions.

### 3. How to implement `do while` in python?
Python does not have a built-in do...while loop like some other languages such as C++ or Java.
However, you can mimic the behavior of a do...while loop using a while loop with a break statement to ensure that the loop executes at least once.
```python
while True:
  # code
  if not condition:
    break
```
### 5.Equivalent of `pass` in Java and C++.
- Python: `pass`
- c++: `{}` (empty block) or `;`
- Java: `{}` (empty block) or `;`

###### c++
  ```c++
  if (condition) {
    // pass equivalent
}
```
```c++
  if (condition) {
    ; // pass equivalent
}
```

###### java
```java
  if (condition) {
    // pass equivalent
}
```
```java
  if (condition) {
    ; // pass equivalent
}
```

  


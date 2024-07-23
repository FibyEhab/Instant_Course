# Task1
---
1. **Pogramming language that support and not support automatic Garbage Collection.**
2. **The 13 principles of clean code.**
3. **How to implement `do while` in python?**
4. **Comparison between `for` and `while` in python.**
5. **Equivalent of `pass` in Java and C++**
---
### Answers:
#### 2. The 13 principles of clean code.
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

#### 3. How to implement `do while` in python?
Python does not have a built-in do...while loop like some other languages such as C++ or Java.
However, you can mimic the behavior of a do...while loop using a while loop with a break statement to ensure that the loop executes at least once.
```python
while True:
  # code
  if not condition:
    break
```
#### 5.Equivalent of `pass` in Java and C++.
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

  


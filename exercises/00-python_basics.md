# Exercises - 00 - Python Basics

## Part 1: Variables & Data Types

1.  **Recall:** Define the four basic data types in Python (Integer, Float, String, and Boolean) and provide an example of each.
2.  **Recall:** What happens if you try to use a variable that has not been defined yet? Identify the specific name of the error Python will raise.
3.  **Understand (Output Prediction):** What is the output of the following code? Explain why the second result is different from the first.
    ```python
    x = 10
    y = "10"
    print(x * 2)
    print(y * 2)
    ```
4.  **Understand (Output Prediction):** Predict the output of this code and explain the concept of string concatenation:
    ```python
    first_name = "Alice"
    last_name = "Wonderland"
    full_name = first_name + " " + last_name
    print(full_name.upper())
    ```
5.  **Apply (Use in Code):** Create variables to store a person's name, age, and whether they are a student or not. Print a single sentence using all three variables.
6.  **Apply (Problem Solving):** Create a program that defines a variable `radius = 5` and `pi = 3.14`. Calculate the area of the circle ($area = \pi r^2$) and store it in a variable called `area`, then print the result.
7.  **Analyze (Change Line):** In the code below, what happens if we change **line 2** to `age = int("25")`? How does this fix the error?
    ```python
    age = "25"
    next_year = age + 1  # Line 2
    print(next_year)
    ```
8.  **Analyze (Change Line):** In the code below, what happens if we change **Line 1** to `x = 5.0`? How does the `type(x)` output change?
    ```python
    x = 5         # Line 1
    print(type(x))
    ```
9.  **Evaluate (Relevance):** Discuss why using meaningful variable names (e.g., `total_cost` vs `x`) is relevant to professional software maintenance and debugging.
10. **Create (Solve Problem):** Write a script that initializes two variables, `a = 5` and `b = 10`. Write code to swap their values so that `a` becomes 10 and `b` becomes 5 **without** typing the numbers directly (Hint: use a temporary variable).

---

## Part 2: Lists

1.  **Recall:** What is the index number of the first item in a Python list? What is the index number of the last item using negative indexing?
2.  **Recall:** Which can be changed after creation: a List or a String?
3.  **Understand (Output Prediction):** What is the output of the following code?
    ```python
    numbers = [10, 20, 30, 40, 50]
    print(numbers[1])
    print(numbers[-1])
    ```
4.  **Understand (Output Prediction):** What is the output of the following slicing operation?
    ```python
    my_list = ['a', 'b', 'c', 'd', 'e', 'f']
    print(my_list[1:4])
    ```
5.  **Apply (Use in Code):** Create a list called `fruits` containing "apple", "banana", and "cherry". Then, write code to add "orange" to the end of the list using a list method.
6.  **Apply (Problem Solving):** Create a list of 5 numbers. Write code that replaces the middle number (index 2) with the number 99 and prints the updated list.
7.  **Analyze (Change Line):** Consider the code below. What happens to the list if we change **line 2** to `data.remove(20)`? Contrast this with what would happen if we used `data.pop(1)`.
    ```python
    data = [10, 20, 30, 20, 40]
    # Line 2: intent is to modify the list
    print(data)
    ```
8.  **Analyze (Change Line):** Given the list `colors = ["red", "green", "blue"]`. What happens if we try to print `colors[3]`? Explain why this specific error occurs.
9.  **Evaluate (Relevance):** Discuss why a List is more relevant than creating individual variables (e.g., `student1`, `student2`...) when storing the test scores of 50 students.
10. **Create (Solve Problem):** Write a program that takes the list `scores = [88, 92, 79, 94, 85]` and calculates the average score using the `sum()` and `len()` functions.

---

## Part 3: For Loops

1.  **Recall:** What are the three parameters you can pass to the `range()` function, and what does each one represent?
2.  **Recall:** What is the purpose of the `break` keyword inside a loop? Give a brief scenario of when it would be used.
3.  **Understand (Output Prediction):** What is the final value of `total` printed at the end of this loop?
    ```python
    total = 0
    for i in range(5):
        total = total + i
    print(total)
    ```
4.  **Understand (Output Prediction):** What is the output of this nested loop?
    ```python
    for x in [1, 2]:
        for y in ['a', 'b']:
            print(x, y)
    ```
5.  **Apply (Use in Code):** Write a `for` loop that iterates through `range(1, 11)` and prints only the even numbers.
6.  **Apply (Problem Solving):** Given a list `prices = [10, 20, 30]`, write a for loop that calculates a 10% tax for each item and prints the final price (original + tax) for each.
7.  **Analyze (Change Line):** In the code below, what happens if we change **line 1** to `for name in guests:` (assuming `guests` is a list of strings)?
    ```python
    for i in range(5): # Line 1
        print("Hello")
    ```
8.  **Analyze (Change Line):** What happens if we change the indentation of **Line 4** to be aligned with `x = n * 2`? How does the output change?
    ```python
    numbers = [1, 2, 3]
    for n in numbers:
        x = n * 2
    print(x) # Line 4
    ```
9.  **Evaluate (Relevance):** Discuss why "For Loops" are relevant to the programming concept of **DRY** (Don't Repeat Yourself). How do they improve code scalability?
10. **Create (Solve Problem):** Write a code that takes a string `word = "Python"` and prints each character in reverse order (from 'n' to 'P') using a for loop.

---

## Part 4: Functions

1.  **Recall:** What is a "docstring" in a Python function? Where is it located, and who is it meant for?
2.  **Recall:** What are typehints and how do they help reading your code?
3.  **Understand (Output Prediction):** What is the output of this code? Focus on how the return value is used.
    ```python
    def add(a, b):
        return a + b

    result = add(5, 3)
    print(result + 10)
    ```
4.  **Understand (Output Prediction):** What is the output of this code? Explain the concept of **Variable Scope**.
    ```python
    x = 50
    def my_func():
        x = 20
        print("Inside:", x)

    my_func()
    print("Outside:", x)
    ```
5.  **Apply (Use in Code):** Define a function called `greet_user` that takes one argument, `name`. It should return the string "Welcome back, [name]!".
6.  **Apply (Problem Solving):** Write a function called `is_positive` that takes a number as an argument. It should return `True` if the number is greater than 0, and `False` otherwise.
7.  **Analyze (Change Line):** What happens if we run the code below, but change **line 4** to `calculate_area(5)`? Why does Python throw a `TypeError`?
    ```python
    def calculate_area(length, width):
        return length * width

    print(calculate_area(5, 4)) # Line 4
    ```
8.  **Analyze (Change Line):** Consider the function below. What happens if we change **line 1** to `def say_hello(name="Guest"):` and then call `say_hello()` without arguments?
    ```python
    def say_hello(name): # Line 1
        print("Hello " + name)
    ```
9.  **Evaluate (Relevance):** Discuss why functions are relevant to collaborative coding. How does modularity help two people work on the same program?
10. **Create (Solve Problem):** Create a function called `celsius_to_fahrenheit` that takes a temperature in Celsius as a parameter and returns the Fahrenheit equivalent. (Formula: $F = (C \times 9/5) + 32$).
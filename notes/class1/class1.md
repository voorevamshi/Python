## 1. Python History & Origins

-   **What is it?** Python is a **general-purpose, high-level** programming language.
    
-   **The Creator:** Developed by **Guido van Rossum** at CWI (National Research Institute) in the Netherlands.
    
-   **Timeline:**
    
    -   Implementation started in **1989**.
        
    -   Official Date of Birth (Release): **February 20, 1991**.
        
-   **The Name:** It wasn't named after the snake! Guido took the name from the popular BBC comedy show **"Monty Python's Flying Circus"** (which aired from 1969 to 1974).
    

## 2. Python's Multi-Paradigm Design (Where it borrowed features)

Python is a "blend" of the best features from various programming languages:

| Feature Borrowed | Source Language |
| :--- | :--- |
| **Functional Programming** | C |
| **Object-Oriented Programming (OOP)** | C++ |
| **Scripting Features** | Perl and Shell script |
| **Modular Programming** | Modula-3 |
| **Syntax** | C and ABC Language |
----------


## 3. Where is Python Used?

Python is incredibly versatile and used across almost every domain in technology:

-   **Desktop & Web Applications** (e.g., Django framework)
    
-   **Database & Networking** applications
    
-   **Games** development
    
-   **Data Analysis, Machine Learning, & AI**
    
-   **Internet of Things (IoT)** applications
    

----------

## 4. Key Takeaways from Code Snippets

### Basic Operations & Dynamic Typing

-   **Printing:** `print("Hello world")` displays text on the screen.
    
-   **Multi-variable Assignment:** Python allows you to assign multiple variables in a single line:
    
    Python
    
    ```
    a, b = 10, 20  # Assigns 10 to a, and 20 to b
    
    ```
    
-   **Dynamic Typing (`type()`):** You don't need to declare the data type in Python. The language automatically detects it based on the value assigned.
    
    -   If `a = 10`, `type(a)` outputs `<class 'int'>` (Integer)
        
    -   If `a = True`, `type(a)` outputs `<class 'bool'>` (Boolean)
        

### Functions & Syntax Rules

-   **Defining Functions:** Functions are created using the `def` keyword.
    
-   **Syntax Error Warning:** Python is highly sensitive to spacing and formatting.
    
    -   ❌ `def f1 (): print("Good Evening")` $\rightarrow$ Spacing before the parentheses can trigger a `SyntaxError`.
        
    -   `def f1(): print("Good Evening")` $\rightarrow$ Correct syntax.
        
-   **Calling a Function:** Once defined, you run a function by typing its name with parentheses: `f1()`.
    

----------

> **Tip for your next class:** Keep an eye out for **indentation** (the spaces at the beginning of a code line). In Python, indentation is not just for readability; it replaces the curly brackets `{}` used in languages like C/C++ to define blocks of code!

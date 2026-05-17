## 1. Flavors of Python

Python comes in different implementations (flavors) tailored for different environments and technologies:

-   **CPython:** The standard, original implementation of Python written in C. It is what you download from python.org.
    
-   **Jython (or JPython):** Designed to run on the Java platform. It compiles Python code directly into Java Bytecode so it can run on a JVM.
    
-   **IronPython:** Designed for Microsoft’s .NET framework and Common Language Runtime (CLR).
    
-   **PyPy:** Known for **high performance**. It replaces the standard PVM with an execution engine containing a **JIT (Just-In-Time) Compiler**, speeding up execution drastically.
    
-   **RubyPython:** A bridge implementation that allows integration between Python and Ruby software.
    
-   **AnacondaPython:** Specifically packaged for **Data Science, Machine Learning, and Big Data**. It comes pre-loaded with thousands of data science libraries.
    
-   **Stackless:** Python optimized for **concurrency** and multithreading. It manages tasks without using the standard C stack, making it highly efficient for parallel processing.
    

----------

## 2. Python Versions & Backward Compatibility

-   **Python 1.0:** Released in January 1994.
    
-   **Python 2.0:** Released in October 2000.
    
-   **Python 3.0:** Released in December 2008.
    

### The "No Backward Compatibility" Rule

In traditional programming, new versions must support old code. However, **Python 3 did not provide backward compatibility for Python 2**. Python 3 was a complete overhaul to fix fundamental design flaws.

> 🛑 **Note:** Support for Python 2 officially ended entirely by **2020**.

### Key Differences (Python 2 vs. Python 3)

| Feature | Python 2 | Python 3 |
| :--- | :--- | :--- |
| **Print Statement** | `print "Hello"` (Valid) | `print("Hello")` (Requires parentheses) |
| **Data Types** | Had both `int` and `long` data types. | `long` was removed. `int` handles large numbers automatically. |


## 3. Identifiers in Python

An **Identifier** is simply a name used to identify a variable, function, class, or module in a program.

-   `x = 10` ($\rightarrow$ `x` is a variable identifier)
    
-   `def f1():` ($\rightarrow$ `f1` is a function identifier)
    
-   `class Test:` ($\rightarrow$ `Test` is a class identifier)
    

### Rules to Define Identifiers

1.  **Allowed Characters:** You can use alphabet symbols (lowercase `a-z`, uppercase `A-Z`), digits (`0-9`), and the underscore (`_`). **No special characters** like `$` are allowed.
    
    -   `cash = 10` (Valid) | `ca$h = 10` (Invalid)
        
2.  **Cannot Start with a Digit:** An identifier can contain numbers, but cannot begin with one.
    
    -   `total123 = 10` (Valid) | `123total = 10` (Invalid)
        
3.  **Case Sensitivity:** Python is case-sensitive. Upper and lowercase identifiers are completely different.
    
    -   `total = 10` and `TOTAL = 20` are treated as two separate variables.
        
4.  **Length:** Length does not matter; it can be as long as needed.
    
5.  **Keywords:** You cannot use reserved keywords (like `def`, `if`, `while`, `class`) as identifier names.
    

### Quick Validity Test (From your class)
| Identifier | Valid / Invalid? | Reason |
| :--- | :--- | :--- |
| `123total` | ❌ Invalid | Starts with a digit. |
| `total123` |  Valid | Contains letters and digits correctly. |
| `java2share` |  Valid | Contains letters and digits correctly. |
| `ca$h` | ❌ Invalid | Contains the special character `$`. |
| `102_abc_abc_` | ❌ Invalid | Starts with a digit. |
| `def` | ❌ Invalid | It is a reserved keyword (used for functions). |
| `if` | ❌ Invalid | It is a reserved keyword (used for conditions). |

## 4. Understanding Underscores (`_` vs `__`)

The use of underscores at the beginning of an identifier changes its meaning and visibility in Python:

-   **Single Underscore (`_variable`):** Indicates that the variable or method is intended for **internal/private use** inside that class or module. It is a gentle warning to other programmers: _"Please don't touch this outside this file."_
    
-   **Double Underscore (`__variable`):** Activates **Name Mangling**. It tells the Python interpreter to strongly protect this variable from being easily accessed or overwritten from outside the class, mimicking a **strictly private** variable.
    
-   **Bonus - Double Leading & Trailing (`__init__`):** These are special system-defined names (often called "dunder" methods). Never name your custom variables this way.

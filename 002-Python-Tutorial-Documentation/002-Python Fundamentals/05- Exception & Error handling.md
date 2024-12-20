### Exception and Error Handling in Python ###

---

Python provides a robust exception-handling mechanism to deal with errors during runtime. Exceptions are objects that represent errors. The main keywords are `try`, `except`, `else`, `finally`, and `raise`.

**Example:**  
```python
try:
    result = 10 / 0  # This will cause a ZeroDivisionError
except ZeroDivisionError as e:
    print(f"An arithmetic error occurred: {e}")
finally:
    print("Execution completed.")
```

---

Key points:
- **try**: The block of code to be tested for errors.
- **except**: The block of code to handle the error.
- **finally**: The block of code that will execute no matter what.
- **raise**: Used to raise an exception manually. 


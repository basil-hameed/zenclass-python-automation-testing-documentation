To create a new `pytest` test file in VS Code:

### **Steps to Create a New `pytest` Test File in VS Code:**

1. **Open VS Code**:
   - Ensure you have Python and `pytest` installed. You can check by running `pytest --version` in the terminal to see the installed version.

2. **Create a New Python File**:
   - Go to File > New File or use `Ctrl+N` (Windows/Linux) or `Cmd+N` (Mac) to open a new Python file.
   - Save the file with a `.py` extension, for example, `test_sample.py`.

3. **Write Your First Test Case**:
   - You can now start writing `pytest` test cases. Here's an example to get started:

```python
# test_sample.py

import pytest

def test_sample():
    assert 1 + 1 == 2
```

4. **Running Tests**:
   - To run the test, open the terminal in VS Code (Terminal > New Terminal) and navigate to the directory containing your test file.
   - Run the test using `pytest`:

   ```bash
   pytest test_sample.py
   ```

5. **Viewing Test Results**:
   - `pytest` will output the test results directly in the terminal. Passed tests will show green, and failed tests will show red.

This setup allows you to start writing and running `pytest` tests quickly in VS Code, similar to how you would with TestNG in Eclipse.
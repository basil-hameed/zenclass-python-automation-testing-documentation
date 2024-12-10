### **Setting Up Visual Studio Code (VS Code) for Python**  
---

**Step 1:**  
Visit the official Visual Studio Code website:  
[https://code.visualstudio.com/](https://code.visualstudio.com/)  

---

**Step 2:**  
Click on the **“Download”** button and select the appropriate version for your operating system (Windows, macOS, or Linux).  

---

**Step 3:**  
Once the installer is downloaded, run the installer and follow the on-screen instructions to complete the installation.  

---

**Step 4:**  
Launch VS Code. On the first run, you may see a "Welcome" screen.  

---

**Step 5:**  
Install the Python extension for VS Code:  

1. Open the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing `Ctrl+Shift+X`.  
2. In the Extensions search bar, type **"Python"**.  
3. Locate the Python extension (published by Microsoft) and click the **Install** button.  

---

**Step 6:**  
Ensure Python is installed on your system. If not, download and install it from the official Python website:  
[https://www.python.org/downloads/](https://www.python.org/downloads/)  

---

**Step 7:**  
Set up Python in VS Code:  

1. Open a Python file or create a new one (`Ctrl+N` and save it with a `.py` extension, e.g., `hello_world.py`).  
2. Press `Ctrl+Shift+P` to open the Command Palette.  
3. Type and select **"Python: Select Interpreter"**.  
4. Choose the Python interpreter you want to use.  

---

### **Writing Your First Python Program in VS Code**  


**Step 1:**  
Create a new Python file in VS Code:  

1. Click **File > New File**.  
2. Save the file with a `.py` extension, such as `hello_world.py`.  

---

**Step 2:**  
Write the following code:  

```python
# File: hello_world.py
def main():
    print("Hello, World!")

if __name__ == "__main__":
    main()
```

---

**Step 3:**  
Run the Python file:  

1. Open the file in VS Code.   
2. Click **"Run"**.  
3. Alternatively, open the terminal and run the file using the command:  
   ```bash
   python hello_world.py
   ```

---
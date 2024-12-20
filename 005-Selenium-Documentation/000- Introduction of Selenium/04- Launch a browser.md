### How to Create a Simple Selenium Project to Launch a Browser in Python ###


**Steps to Create and Launch a Browser Using Selenium in Python:**


### 1. Set Up Selenium Environment
- Install Python and Selenium as detailed [here](#Installation-of-Selenium).

---

### 2. Create a Python Project
1. **Create a Folder for the Project:**
   - Name the folder (e.g., `Selenium_Project`).

2. **Set Up the Python Script:**
   - Inside the folder, create a new Python script file (e.g., `launch_browser.py`).

---

### 3. Write the Python Script
1. **Set Up WebDriver Properties:**
   In Selenium Python, you don't need to manually set system properties like Java. Instead, you pass the driver path directly to the WebDriver.

2. **Example Script:**
   ```python
   from selenium import webdriver
   from selenium.webdriver.common.by import By

   # Specify the path to the WebDriver
   driver_path = "path_to_your_chromedriver"

   # Initialize the WebDriver (Chrome in this case)
   driver = webdriver.Chrome(executable_path=driver_path)

   # Launch the URL
   driver.get("https://www.google.com")

   # Print the title of the webpage
   print("Title of the page is:", driver.title)

   # Close the browser
   driver.quit()
   ```

---

### 4. Using `webdriver-manager` (Optional)
To avoid managing WebDriver manually, use the **`webdriver-manager`** library:
```bash
pip install webdriver-manager
```

**Updated Script with WebDriver-Manager:**
```python
from selenium import webdriver
from webdriver_manager.chrome import ChromeDriverManager

# Automatically fetch and use the correct ChromeDriver version
driver = webdriver.Chrome(ChromeDriverManager().install())

# Launch the URL
driver.get("https://www.google.com")

# Print the title of the webpage
print("Title of the page is:", driver.title)

# Close the browser
driver.quit()
```

---

### 5. Execute the Script
Run the script from your terminal or IDE:
```bash
python launch_browser.py
```

---

**Key Points in Python (Compared to Java):**
- No need to use `System.setProperty`.
- WebDriver setup and initialization are simpler.
- The script is more concise and Pythonic.

Your browser should now launch successfully with the specified URL!
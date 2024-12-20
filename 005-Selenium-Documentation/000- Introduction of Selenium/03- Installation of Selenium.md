### Installation of Selenium in Python ###

---

**Steps to Set Up Selenium in Python:**

---

### 1. Install Python
- Ensure Python is installed on your system. Download it from [Python's official website](https://www.python.org/).  
- Verify installation:
  ```bash
  python --version
  ```

---

### 2. Install Selenium Library
- Install the Selenium package using pip:
  ```bash
  pip install selenium
  ```
- Verify installation:
  ```bash
  pip show selenium
  ```

---

### 3. Download Browser Drivers
Selenium requires browser drivers to interact with browsers like Chrome, Firefox, Edge, etc.

#### Steps for ChromeDriver:
1. Open [ChromeDriver Downloads](https://chromedriver.chromium.org/downloads).
2. Check your Chrome version:
   - Open Chrome.
   - Go to `Settings > About Chrome`.
   - Note the version number.
3. Download the ChromeDriver version matching your browser version.
4. Extract the downloaded file and note the path to the `chromedriver` executable.

---

### 4. Set Up Your Selenium Project
Create a project folder for your Selenium scripts.

---

### 5. Basic Selenium Script Example
Save the following script in your project directory as `test.py`:
```python
from selenium import webdriver

# Specify the path to the ChromeDriver executable
driver_path = "path_to_your_chromedriver"

# Initialize the WebDriver
driver = webdriver.Chrome(executable_path=driver_path)

# Open a website
driver.get("https://www.google.com")

print("Title of the page is:", driver.title)

# Close the browser
driver.quit()
```

---

### 6. Run the Selenium Script
- Execute the script using Python:
  ```bash
  python test.py
  ```

---

### 7. Optional: Manage Drivers Automatically
Instead of manually downloading and managing drivers, use the **webdriver-manager** package:
```bash
pip install webdriver-manager
```

**Updated Script Using `webdriver-manager`:**
```python
from selenium import webdriver
from webdriver_manager.chrome import ChromeDriverManager

# Automatically fetch and use the correct ChromeDriver version
driver = webdriver.Chrome(ChromeDriverManager().install())

# Open a website
driver.get("https://www.google.com")

print("Title of the page is:", driver.title)

# Close the browser
driver.quit()
```

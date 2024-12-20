### Locator Strategies in Selenium with Python ###

**Locators in Selenium**:
Locators are used to find web elements on a webpage. There are multiple locators available in Selenium to locate elements:

---

### 1. **ID Locator**:
- **Fastest locator** in Selenium.
- **Syntax**: `driver.findElement(By.ID("id_value"));`
- **Example**:
  ```python
  usernameInput = driver.findElement(By.ID("username"));
  ```

---

### 2. **Class Name Locator**:
- Used to locate elements by their class name attribute.
- **Syntax**: `driver.findElement(By.CLASS_NAME("class_name"));`
- **Example**:
  ```python
  loginButton = driver.findElement(By.CLASS_NAME("login-button"));
  ```

---

### 3. **Name Locator**:
- Locates elements by their `name` attribute.
- **Syntax**: `driver.findElement(By.NAME("name_value"));`
- **Example**:
  ```python
  usernameInput = driver.findElement(By.NAME("username"));
  ```

---

### 4. **Xpath Locator**:
- Provides a path to locate an element.
- **Syntax**: `driver.findElement(By.XPATH("xpath_value"));`
- **Example**:
  ```python
  submit = driver.findElement(By.XPATH("//button[@id='submit']"));
  ```

---

### 5. **CSS Selector Locator**:
- Allows for selecting elements using a CSS selector.
- **Syntax**: `driver.findElement(By.CSS_SELECTOR("css_selector_value"));`
- **Example**:
  ```python
  submit = driver.findElement(By.CSS_SELECTOR("button.login-button"));
  ```

---

### 6. **Tag Name Locator**:
- Locates elements based on their tag name.
- **Syntax**: `driver.findElement(By.TAG_NAME("tag_name"));`
- **Example**:
  ```python
  inputField = driver.findElement(By.TAG_NAME("input"));
  ```

---

### 7. **Link Text Locator**:
- Used for locating links directly by their text.
- **Syntax**: `driver.findElement(By.LINK_TEXT("link_text"));`
- **Example**:
  ```python
  forgotPasswordLink = driver.findElement(By.LINK_TEXT("Forgot Password?"));
  ```

---

### 8. **Partial Link Text Locator**:
- Locates links that partially match the link text.
- **Syntax**: `driver.findElement(By.PARTIAL_LINK_TEXT("partial_link_text"));`
- **Example**:
  ```python
  forgotPasswordLink = driver.findElement(By.PARTIAL_LINK_TEXT("Forgot"));
  ```

###  Methods in Selenium with Python ###


**Selenium WebElement Methods**: These methods allow you to interact with web elements on a webpage, such as buttons, input fields, and links. Each method serves a specific purpose:

---

### 1. **click()**:
- **Purpose**: Simulates a mouse click on a web element (e.g., button, link, checkbox).
- **Syntax**:
  ```python
  button = driver.findElement(By.ID("myButton"));
  button.click();
  ```
- **Example**: Clicking a button with the id "myButton".

---

### 2. **sendKeys()**:
- **Purpose**: Simulates typing into an input field or any editable element on a webpage.
- **Syntax**:
  ```python
  inputField = driver.findElement(By.ID("username"));
  inputField.sendKeys("myusername");
  ```
- **Example**: Typing the text "myusername" into an input field.

---

### 3. **clear()**:
- **Purpose**: Clears the text present in an input field or textarea.
- **Syntax**:
  ```python
  inputField = driver.findElement(By.ID("username"));
  inputField.clear();
  ```
- **Example**: Clearing the text in the input field with the id "username".

---

### 4. **submit()**:
- **Purpose**: Submits a form by emulating the user’s click on the submit button or pressing the Enter key on the keyboard.
- **Syntax**:
  ```python
  form = driver.findElement(By.ID("loginForm"));
  form.submit();
  ```
- **Example**: Submitting a form with the id "loginForm".

---

### 5. **getText()**:
- **Purpose**: Retrieves the visible (rendered) text of a web element.
- **Syntax**:
  ```python
  heading = driver.findElement(By.TAG_NAME("h1"));
  headingText = heading.getText();
  print("Heading: " + headingText);
  ```
- **Example**: Getting the text of an `h1` heading.

---

### 6. **getAttribute()**:
- **Purpose**: Retrieves the value of a specified attribute of a web element.
- **Syntax**:
  ```python
  link = driver.findElement(By.TAG_NAME("a"));
  hrefValue = link.getAttribute("href");
  print("Link URL: " + hrefValue);
  ```
- **Example**: Retrieving the `href` attribute of a link.

---

### 7. **isDisplayed(), isEnabled(), isSelected()**:
- **Purpose**:
  - **isDisplayed()**: Checks if the element is currently visible on the page.
  - **isEnabled()**: Checks if the element is enabled (e.g., not disabled).
  - **isSelected()**: Checks if the element is selected (applicable for checkboxes, radio buttons).
- **Syntax**:
  ```python
  element = driver.findElement(By.ID("myElement"));
  isVisible = element.isDisplayed();
  isEnabled = element.isEnabled();
  isSelected = element.isSelected();
  ```

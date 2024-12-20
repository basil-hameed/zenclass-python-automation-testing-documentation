## Frame: ##

Frame allow dividing a browser window into multiple sections, each with its own HTML document. Selenium needs to switch to the frame in which the target element is present to interact with it.

### **Example Code**:
```python
# Click a button that opens a new window
newWindowButton = driver.find_element(By.ID, "newWindowButton")
newWindowButton.click()

# Get all window handles
windowHandles = driver.window_handles
originalWindowHandle = driver.current_window_handle

# Switch to the new window
for handle in windowHandles:
    if handle != originalWindowHandle:
        driver.switch_to.window(handle)
        
        # Perform actions on the new window
        # Example: Locate an element and input text
        newWindowElement = driver.find_element(By.ID, "newWindowElement")
        newWindowElement.send_keys("Some text")

        break

# Switch back to the original window if needed
driver.switch_to.window(originalWindowHandle)
```

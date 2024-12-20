## Installing Pytest in Visual Studio Code (VSCode) ##

To install Pytest in Visual Studio Code, follow these steps:

### Method 1: Installing via VSCode UI

1. **Open Visual Studio Code**:
   - Launch Visual Studio Code on your computer.

2. **Open Extensions View**:
   - Click on the `Extensions` icon on the left sidebar or press `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac).

3. **Search for Pytest**:
   - In the Extensions search bar, type `pytest`.
   - Press `Enter` or click the search icon.

4. **Install Pytest**:
   - In the search results, locate the `pytest` extension. It may be from `Microsoft` or `Python Extension Pack for Visual Studio Code`.
   - Click on the `Install` button next to the `pytest` extension.

5. **Verify Installation**:
   - After installation, you can verify by opening a Python file and checking if `pytest` is recognized as a valid testing tool. You should be able to run tests directly from the terminal in VSCode.

### Method 2: Installing via Command Line

Alternatively, you can install Pytest directly from the VSCode terminal:

1. **Open Integrated Terminal in VSCode**:
   - Go to the `View` menu and select `Terminal` or press `Ctrl+` (`Cmd+`) ```.

2. **Install Pytest**:
   - Run the following command:
     ```bash
     pip install pytest
     ```

3. **Verify Installation**:
   - Open a Python file and run a basic Pytest command like `!pytest` to verify that it runs without errors.
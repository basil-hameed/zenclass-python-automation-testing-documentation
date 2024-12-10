### Installation Guide (Python)  


**Step 1:**  
---  
Open the [https://www.python.org/downloads/](https://www.python.org/downloads/) URL in your browser. It will navigate to the official Python downloads page.

**Step 2:**  
---  
- Select the version of Python you want to download.  
- Select the operating system.  
- Scroll down to the page and click on the download link suitable for your computer’s operating system. For a 64-bit machine, choose the file ending with **x64**.

**Step 3:**  
---  
Once the download is complete, run the installer.

**Step 4:**  
---  
When the Python installation wizard opens, make sure to check the box **Add Python to PATH** before clicking on the **Install Now** button.

**Step 5:**  
---  
The installation process will be started.

**Step 6:**  
---  
Once the installation completes, click on the **Close** button.
---


### Setting up Environment in Python  


After downloading Python, you need to configure the environment variables for Python.

**Step 1:**  
---  
Locate the Python installation folder:  
By default, Python is installed in the **`C:\Users\<YourUsername>\AppData\Local\Programs\Python\Python<Version>`** folder. In case you have installed Python at another location, copy that path.



**Step 2:**  
---  
Go to the search bar and search for **Environment Variables -> Edit the system environment variables.** Under the **Advanced** tab, click on **Environment Variables**.



**Step 3:**  
---  
In the Environment Variables window, locate the **Path** variable under **System variables**, and click the **Edit** button.



**Step 4:**  
---  
In the Path variable, click on **New** and add the folder path where Python is installed (e.g., **`C:\Users\<YourUsername>\AppData\Local\Programs\Python\Python<Version>`**). 



**Step 5:**  
---  
Click **OK** to save the changes. To verify the installation, open **Command Prompt** and type:  
```bash
python --version
```
If Python is installed correctly, the version will be displayed.

---  
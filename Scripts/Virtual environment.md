
# Setting up Virtual Environment for Jupyter Notebooks in Visual Studio Code

This guide will help you set up a virtual environment for Jupyter Notebooks in Visual Studio Code. Using a virtual environment ensures that your project dependencies are isolated from other projects and system-wide packages.

## Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/) installed on your system.
- Python installed on your system.
- You can as well install anaconda from [here](https://www.anaconda.com/)
  

## Steps

1. **Install Visual Studio Code**:

   Make sure you have Visual Studio Code installed on your system. You can download it from the official website: [Visual Studio Code](https://code.visualstudio.com/).

2. **Install Python Extension**:

   Inside VSCode, install the Python extension by Microsoft. This extension provides support for Python development in Visual Studio Code, including debugging, linting, IntelliSense, code navigation, code formatting, and more.

3. **Create a New Folder for Your Project**:

   Create a new folder on your system where you want to store your Jupyter Notebooks and associated files.

4. **Open the Folder in VSCode**:

   Open Visual Studio Code and navigate to the newly created folder using the File > Open Folder option.

5. **Open a Terminal in VSCode**:

   Press `Ctrl+`` to open the integrated terminal in VSCode. This terminal will be used to run commands.

6. **Create a Virtual Environment**:

   In the terminal, run the following command to create a virtual environment (replace `myenv` with the name you want for your virtual environment):

   ```
   python3 -m venv myenv
   ```

7. **Activate the Virtual Environment**:

   Depending on your operating system, activate the virtual environment:

   - **Windows**:

     ```
     .\myenv\Scripts\activate
     ```

   - **Mac/Linux**:

     ```
     source myenv/bin/activate
     ```

8. **Install Jupyter Notebooks**:

   While the virtual environment is active, install Jupyter Notebooks using pip:

   ```
   pip install jupyter
   ```

9. **Launch Jupyter Notebooks**:

   To launch Jupyter Notebooks, run the following command in the terminal:

   ```
   jupyter notebook
   ```

10. **Create or Open a Notebook**:

    In the Jupyter Notebook interface that opens in your default web browser, you can create a new notebook or open an existing one.

11. **Start Coding**:

    You can now start coding in your Jupyter Notebook environment within VSCode.

Remember to deactivate the virtual environment when you're done working:

- **Windows**:

  ```
  deactivate
  ```

- **Mac/Linux**:

  ```
  deactivate
  ```



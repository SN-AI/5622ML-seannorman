# Environment Setup

This document describes how to set up the Python virtual environment required to run the Jupyter notebook (`model-notebook.ipynb`) in this project. Using a virtual environment ensures that all dependencies are managed correctly and consistently across different machines.

## Prerequisites

*   **Python 3:** Ensure you have Python 3 installed on your system. You can download it from [python.org](https://www.python.org/). Verify the installation by opening a terminal or command prompt and running `python3 --version` (macOS/Linux) or `python --version` (Windows).
*   **Git:** You need Git to clone the repository if you haven't already.

## Setup Steps

1.  **Clone the Repository (if needed):**
    If you haven't already, clone the project repository to your local machine:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Run the Setup Script:**
    Navigate to the project's root directory in your terminal or command prompt. Choose the script appropriate for your operating system:

    *   **macOS / Linux:**
        *   Make the script executable (you only need to do this once):
          ```bash
          chmod +x setup.sh
          ```
        *   Run the script:
          ```bash
          ./setup.sh
          ```

    *   **Windows:**
        *   Run the batch script:
          ```bat
          setup.bat
          ```
    This script will create a virtual environment folder named `.venv` and install all the necessary Python packages listed in `requirements.txt`.

3.  **Activate the Virtual Environment:**
    After the setup script finishes, you need to activate the environment in your terminal session:

    *   **macOS / Linux:**
        ```bash
        source .venv/bin/activate
        ```
        Your terminal prompt should now show `(.venv)` at the beginning.

    *   **Windows (Command Prompt):**
        ```bat
        .\.venv\Scripts\activate.bat
        ```
        Your command prompt should now show `(.venv)` at the beginning.

    *   **Windows (PowerShell):**
        ```powershell
        .\.venv\Scripts\Activate.ps1
        ```
        *(Note: You might need to adjust your PowerShell execution policy if you encounter issues: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process`)*

4.  **Using the Environment:**
    *   Once activated, any Python or pip commands (`python`, `pip`, `jupyter`) will use the versions installed within the `.venv` environment.
    *   You can now run `jupyter notebook` to start the Jupyter server or open the `model-notebook.ipynb` file in VS Code.
    *   VS Code should automatically detect the `.venv` environment. If not, you can manually select it using the Python interpreter selector (usually in the bottom status bar or via the Command Palette: `Python: Select Interpreter`).

5.  **Deactivating the Environment:**
    When you are finished working, you can deactivate the environment by simply running:
    ```bash
    deactivate
    ```
    This command works on all operating systems.

This setup ensures that your project runs with the specific package versions defined in `requirements.txt`, making it reproducible for anyone using the project.

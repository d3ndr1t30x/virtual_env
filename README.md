
# Python Virtual Environment Setup and Dependency Installation on Kali Linux

This document provides step-by-step instructions for deactivating, deleting, creating a new Python virtual environment, and installing dependencies on Kali Linux.

## Step 1: Deactivate the Python Virtual Environment
If your virtual environment is currently active, deactivate it by running:
```bash
deactivate
```

## Step 2: Delete the Virtual Environment
Navigate to the directory where your virtual environment is located, and delete it. Assuming your virtual environment is named `emailfinder-env`, you can delete it as follows:
```bash
rm -rf emailfinder-env
```

## Step 3: Create a New Python Virtual Environment
Navigate to the directory where you want to create the new virtual environment, and run:
```bash
python3 -m venv emailfinder-env
```

## Step 4: Activate the New Virtual Environment
Once the virtual environment is created, activate it using:
```bash
source emailfinder-env/bin/activate
```

You should now see the virtual environment name (e.g., `(emailfinder-env)`) in your terminal prompt.

## Step 5: Install Dependencies for the Tool
If you have a `requirements.txt` file, install the dependencies as follows:
```bash
pip install -r requirements.txt
```

Alternatively, manually install the dependencies for your tool (e.g., `requests`, `lxml`, `beautifulsoup4`):
```bash
pip install requests lxml beautifulsoup4
```

## Step 6: Verify Installation
List the installed packages in the virtual environment to verify:
```bash
pip list
```

## Step 7: Run the Tool
Once the dependencies are installed, you can run your Python tool as usual.

## Optional: Deactivating the Virtual Environment
When you're done, deactivate the virtual environment by running:
```bash
deactivate
```

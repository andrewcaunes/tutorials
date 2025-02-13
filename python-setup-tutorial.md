# Getting Started with Python Development: A Complete Guide for Beginners

## Introduction

This guide will help you set up your Python development environment and understand the basics of running Python code. We'll cover everything from installing Python to using professional development tools that will make your coding journey easier.

## Part 1: Understanding Python

### What is Python?

Python is a programming language that needs to be installed on your computer to run Python code. Think of it like a translator that converts the code you write into instructions your computer can understand.

### Running Python Code

There are two main ways to run Python code:

1. **Interactive Mode (Python Shell)**
   - Open a terminal (Command Prompt in Windows, Terminal in macOS/Linux)
   - Type `python` and press Enter
   - You'll see a prompt (`>>>`) where you can type Python commands
   - This is great for quick experiments and learning

2. **Running Python Files**
   - Create a file with `.py` extension (e.g., `my_program.py`)
   - Open terminal and navigate to the file's location
   - Run: `python my_program.py`

### Understanding File Paths

When working with Python, understanding file paths is crucial:

- **Absolute paths** start from the root of your system:
  - Windows: `C:\Users\YourName\Documents\project\script.py`
  - Mac/Linux: `/home/YourName/Documents/project/script.py`

- **Relative paths** start from your current location:
  - If you're in `/home/YourName/Documents` and your file is in `project/script.py`
  - You can just use `python project/script.py`

**Important:** When your code needs to access other files (like images or data):
```python
# If your structure is:
# project/
#   ├── script.py
#   └── images/
#       └── flower.png

# In script.py:
image_path = "images/flower.png"  # Relative to where you run the script
```

## Part 2: Setting Up Your Development Environment

### Installing Python with Miniconda

Miniconda is recommended because it:
- Provides Python
- Includes conda for managing virtual environments
- Has a smaller installation size than Anaconda

Installation steps:
1. Download Miniconda from [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
2. Run the installer
3. Open a new terminal window to verify installation with `conda --version`

### Understanding Virtual Environments

A virtual environment is like a clean room for your Python projects:
- Prevents conflicts between different projects
- Makes your projects portable
- Keeps your system Python clean

Basic conda commands:
```bash
# Create a new environment
conda create -n my_project python=3.9

# Activate the environment
conda activate my_project

# Install packages
pip install numpy pandas

# Deactivate when done
conda deactivate
```

### Setting Up Visual Studio Code (VSCode)

VSCode is recommended because it offers:
- Intelligent code completion
- Built-in terminal
- Debugging tools
- Git integration
- Extensive extension ecosystem

Installation and setup:
1. Download from [https://code.visualstudio.com](https://code.visualstudio.com)
2. Install the "Python" extension from Microsoft
3. Install "Pylance" for better code intelligence

Essential VSCode features for Python:
- Code formatting (right-click > Format Document)
- Integrated terminal (Ctrl+` or Cmd+`)
- File explorer (Ctrl+Shift+E or Cmd+Shift+E)
- Command palette (Ctrl+Shift+P or Cmd+Shift+P)

## Part 3: Workflow Example - Starting a New Project

1. **Set Up the Environment**
   ```bash
   # Create and activate environment
   conda create -n my_project python=3.9
   conda activate my_project
   ```

2. **Create Project Directory**
   ```bash
   # Create and navigate to project folder
   mkdir my_project
   cd my_project
   ```

3. **Open VSCode**
   ```bash
   # Open VSCode in current directory
   code .
   ```

4. **Configure VSCode**
   - Select Python interpreter:
     - Press Ctrl+Shift+P (Cmd+Shift+P on Mac)
     - Type "Python: Select Interpreter"
     - Choose your conda environment

5. **Start Coding**
   - Create new file: `hello.py`
   - Write code
   - Run using:
     - Terminal command: `python hello.py`
     - VSCode Run Python File command (Ctrl+F5)

## Next Steps

Once you're comfortable with these basics, consider learning:
- Writing and organizing larger Python programs
- Using Git for version control
- Testing your code
- Using debugging tools in VSCode

Remember: Start small, practice regularly, and don't hesitate to ask for help when needed.

# Python, Virtual Environments, and Flask Setup

This guide will walk you through downloading Python, creating a virtual environment, and installing Flask. It also explains **what all of these tools are** and **why we use them** for web development.

---

## What is Python?

**Python** is a beginner-friendly programming language that we’ll use to build the backend (server-side) of our website. It's powerful, readable, and widely used.

---

## What is a Virtual Environment (venv)?

A **virtual environment** is a separate “box” where you install Python packages for just one project. It keeps your dependencies clean and avoids breaking other projects on your computer.

Think of it like a sandbox for code.

---

## Step 1: Install Python

### Windows / Mac:
- Go to the official Python site: https://www.python.org/downloads/
- Download the latest version (3.x)
- **Windows only:** During install, make sure to check the box that says **"Add Python to PATH"**

### Check if it worked:
Open your terminal and run:

    python --version
or

    python3 --version
You should see something like: `Python 3.11.x`

## Step 2: Create a Virtual Environment (venv)
Navigate to your project folder in the command terminal. 

    cd /[YourFilePath]/NoComplyPress/
then run `python3 -m venv venv` or `python -m venv venv`
This creates a new folder called `venv/` that holds your virtual environment.

## Step 3: Activate the venv
#### Windows Command Prompt

    venv\Scripts\activate

#### Windows Powershell

    .\venv\Scripts\Activate.ps1
Once your python is activate you will see your command terminal look something like `(venv) nate@laptop NoComplyPress %`. This means that it is running successfully and you can now install the python project requirements such as pip and flask. 

## Step 4: Install Flask

Flask is a package used by python that is required for our project. Run the line below

    pip install flask
If this returns an error, you may need to install pip but pip should already come with python. If you run into issues dont be scared to rely on chatGTP for assistance or Youtube tutorials.

## Deactivate venv
simply type the command below to deactivate your venv

    deactivate

As we go along through the project we will need to install new packages but we will let future us worry about that.


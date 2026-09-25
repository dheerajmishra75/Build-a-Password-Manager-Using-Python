# Password Manager Using Python

A simple command-line password manager built with Python for storing and retrieving website passwords.

The project uses a text file for local storage and provides options to save passwords, retrieve passwords, and copy retrieved passwords to the clipboard.

## 🎥 Preview

[▶️ Watch Project Demo](./Preview/Build%20a%20Password%20Manager%20Using%20Python.mp4)

The preview demonstrates saving a website password, retrieving a stored password, and copying the retrieved password to the clipboard.

## ✨ Features

- Command-line password manager
- Save website passwords
- Retrieve passwords using a website name
- Local text-file storage
- Search stored credentials by website
- Copy retrieved passwords to the clipboard
- Simple menu-driven interface
- Handles websites that are not found
- Provides save and retrieval feedback

## 🎯 Project Overview

The Password Manager is a beginner-level Python project focused on practicing file handling, functions, user input, searching, and clipboard operations.

The application stores website-password pairs inside a local `passwords.txt` file.

The program provides three main options:

    1. Save Password
    2. Get Password
    3. Exit

When retrieving a password, the application searches the stored records for the requested website and copies the matching password to the clipboard.

## 🔄 How It Works

    1. The program imports `pyperclip` and `os`.
    2. A `passwords.txt` file is used for local storage.
    3. The user selects an option from the Password Manager menu.
    4. For saving, the user enters a website and password.
    5. The website-password pair is appended to the text file.
    6. For retrieval, the user enters a website.
    7. The program reads the stored records line by line.
    8. It searches for the requested website.
    9. If found, the password is extracted.
    10. `pyperclip` copies the password to the clipboard.
    11. If the website is not found, an appropriate message is displayed.

## 🗂️ Password Storage

The project uses a local file named:

    passwords.txt

Website-password information is stored as text records using a delimiter between the website and password.

Example structure:

    website||password

This provides a simple way for the program to separate the website from the stored password when retrieving credentials.

## 📋 Application Menu

The command-line application provides:

    Password Manager

    1. Save Password
    2. Get Password
    3. Exit

The user enters the corresponding menu option to perform an operation.

## 💾 Save Password

The `save_password()` function:

- Requests the website name
- Requests the password
- Opens `passwords.txt` in append mode
- Writes the website and password
- Displays a successful save message

## 🔎 Get Password

The `get_password()` function:

- Requests the website name
- Opens `passwords.txt`
- Reads stored records
- Searches for the requested website
- Extracts the corresponding password
- Copies the password to the clipboard
- Displays a message when the website is not found

## 📋 Clipboard Support

The project uses the `pyperclip` library to copy retrieved passwords to the system clipboard.

This allows the user to retrieve a stored password without manually selecting and copying it from the text file.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Application development |
| `pyperclip` | Copying passwords to the clipboard |
| `os` | Basic operating-system interaction |
| Text File | Local password storage |
| Functions | Organizing application operations |
| File Handling | Saving and retrieving credentials |

## 📁 Project Structure

    Build-a-Password-Manager-Using-Python/
    │
    ├── Preview_video/
    │   └── Build a Password Manager Using Python.mp4
    │
    ├── main.py
    ├── passwords.txt
    │
    └── README.md

## ▶️ Run Locally

### 1. Clone the Repository

    git clone https://github.com/dheerajmishra75/Build-a-Password-Manager-Using-Python.git

### 2. Navigate to the Project

    cd Build-a-Password-Manager-Using-Python

### 3. Install the Required Package

    pip install pyperclip

### 4. Run the Application

    python main.py

## 🧪 Example Workflow

    Start Application
          ↓
    Password Manager Menu
          ↓
    Choose Save Password
          ↓
    Enter Website
          ↓
    Enter Password
          ↓
    Save to passwords.txt

    OR

    Choose Get Password
          ↓
    Enter Website
          ↓
    Search passwords.txt
          ↓
    Password Found
          ↓
    Copy Password to Clipboard

## 📚 Python Concepts Practiced

- Functions
- User input
- File handling
- Reading text files
- Appending to text files
- String processing
- Lists and iteration
- Conditional statements
- Searching text data
- Exception-aware application flow
- External Python packages
- Clipboard interaction

## 🎯 Learning Outcomes

Through this project, I practiced how to:

- Work with persistent local text-file storage
- Create menu-driven command-line applications
- Read and write text files using Python
- Search stored records
- Extract information from strings
- Use external Python packages
- Interact with the system clipboard
- Organize application functionality into functions

## 🚀 Future Improvements

Possible improvements for future versions include:

- Password encryption
- Master-password authentication
- Secure password hashing
- Password generation
- Better credential storage
- Search improvements
- Delete and update operations
- Database-based storage
- GUI interface
- Secure secret management

## ⚠️ Security Notice

This project is a learning exercise and **should not be used to store real passwords**.

The current implementation stores passwords as plain text in `passwords.txt` and does not provide encryption or a master-password security layer.

For real-world password management, credentials should be protected using established secure storage and encryption practices.

## 🔗 Project Links

- GitHub: https://github.com/dheerajmishra75/Build-a-Password-Manager-Using-Python

## 👨‍💻 Author

**Dheeraj Mishra**

B.Tech CSE Student | Python | Data Science | Machine Learning | Backend Development

## 📌 Disclaimer

This project was created for educational and practice purposes. It is not intended to provide secure production-grade password management.

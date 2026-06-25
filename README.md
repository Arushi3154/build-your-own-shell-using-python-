# build-your-own-shell-using-python-
# Python Custom Shell

A lightweight, interactive command-line interface (CLI) shell built entirely in Python. This project demonstrates core operating system concepts, including process execution, standard input/output stream management, and environment variable parsing.

## 🚀 Features

* **Custom Prompt:** Features an interactive `$ ` prompt that waits for user input.
* **Built-in Commands:**
    * `echo`: Prints the provided arguments back to the standard output.
    * `type`: Identifies whether a command is a shell built-in or an external executable, and provides the file path if it's external.
    * `exit`: Cleanly terminates the shell process.
* **External Program Execution:** Parses the system's `PATH` environment variable to locate and execute external commands (e.g., `ls`, `cat`, `pwd`) using Python's `subprocess` module.
* **Robust Error Handling:** Gracefully handles empty inputs, unknown commands, and `EOF` signals (like `Ctrl+D`) without crashing.

## 🛠️ Prerequisites

* Python 3.x installed on your system.
* A Unix-like environment (Linux/macOS) is recommended for full `PATH` resolution compatibility, though basic built-ins will work on Windows.

## 💻 How to Run

1.  Clone this repository to your local machine:
    ```bash
    git clone [https://github.com/Arushi3154/build-your-own-shell-using-python-.git](https://github.com/Arushi3154/build-your-own-shell-using-python-.git)
    ```
2.  Navigate into the project directory:
    ```bash
    cd build-your-own-shell-using-python-
    ```
3.  Execute the main Python script:
    ```bash
    python3 main.py
    ```

## 📖 Usage Examples

Once the shell is running, you can interact with it just like a standard terminal.

**Using built-in commands:**
```bash
$ echo Hello, World!
Hello, World!

$ type echo
echo is a shell builtin

$ type cat
cat is /bin/cat

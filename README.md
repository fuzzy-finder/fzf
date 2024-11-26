# fzf

**fzf** is a powerful command-line fuzzy finder that allows you to search, filter, and select from a list of items in an interactive way. Whether you're navigating through files, directories, or searching within the output of other commands, fzf provides a fast and intuitive interface to help you find what you're looking for. It is particularly useful for developers, system administrators, and power users who work extensively in the terminal.

fzf is designed to be fast and flexible, and it integrates seamlessly with various shell environments, allowing you to use it as part of your daily workflow.

## Key Features

- **Fuzzy search:** fzf allows you to quickly search through large sets of data, whether it's files, directories, or any list of items. As you type, fzf continuously filters the list based on your input.
- **Live preview:** fzf can show a live preview of the selected file or item (e.g., contents of a file, or a git commit message) to give you additional context before making your selection.
- **Integration with shell commands:** fzf can be easily combined with any shell command, including `find`, `git`, `ps`, `history`, and more, to filter and interact with their output.
- **Customizable keybindings:** fzf allows you to set custom keybindings, making it easy to integrate into your existing workflows.
- **Works with any shell:** fzf works with most modern shells, including Bash, Zsh, Fish, and others, allowing you to use it across various environments.
- **Interactive and intuitive UI:** fzf offers a clean, user-friendly interface that works within the terminal, allowing you to interact with the list of items using a simple set of commands.
- **Cross-platform support:** fzf works on Linux, macOS, and Windows (via WSL or Cygwin), making it a great tool for users across different platforms.

## Installation

### Linux

On Linux, fzf can be installed using a package manager or by using a script.

1. **Using package managers**:
    - **Debian/Ubuntu-based systems**:
        ```bash
        sudo apt install fzf
        ```
    - **Fedora**:
        ```bash
        sudo dnf install fzf
        ```
    - **Arch Linux**:
        ```bash
        sudo pacman -S fzf
        ```

2. **Using the install script**:
    You can also install fzf using the provided installation script:
    ```bash
    git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
    ~/.fzf/install
    ```

### macOS

For macOS, fzf can be installed using Homebrew:

1. **Using Homebrew**:
    ```bash
    brew install fzf
    ```

2. **Install via Git**:
    Alternatively, you can install fzf by cloning the repository:
    ```bash
    git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
    ~/.fzf/install
    ```

### Windows

For Windows, fzf can be installed via **Windows Subsystem for Linux (WSL)** or by using **Cygwin**. Another option is to use **Chocolatey**:

1. **Using Chocolatey**:
    ```bash
    choco install fzf
    ```

2. **WSL or Cygwin**:
    Follow the Linux installation instructions above for WSL or Cygwin environments.

## Usage

Once installed, fzf can be used in a variety of ways. Below are some common use cases.

### File Finder

To search for files in a directory and select one interactively, simply run:

```bash
fzf

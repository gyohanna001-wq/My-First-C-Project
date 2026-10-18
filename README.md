# ❤️ I Love GD! — My First C Program

## 📌 About the Project

Welcome to my **I Love GD!** project!

This is a simple beginner-friendly program written in the C programming language. It displays two messages on the screen:

- `I love GD!`
- `It's really great!`

The purpose of this project is to learn the basics of C programming, understand how to write code, and discover how to run a program on a computer.

## 🎯 Project Goals

- Learn the basics of C.
- Understand how to write a simple program.
- Learn how to display text using `printf()`.
- Understand how to compile and run C code.
- Practice using a code editor and terminal.
- Learn how to share a programming project on GitHub.

## 💻 What Is C?

C is a programming language used to create many types of software, including operating systems, embedded systems, and performance-focused applications.

It is a great language for learning important programming concepts, such as variables, functions, loops, and conditions.

## 🧰 What You Need

Before starting, you will need:

1. A computer running Windows, macOS, or Linux.
2. A code editor, such as Visual Studio Code.
3. A C compiler, such as GCC.
4. Basic knowledge of typing and saving files.

**Important:** Visual Studio Code is a code editor. You also need a C compiler to compile and run C programs.

## 📥 Step 1: Install Visual Studio Code

Visual Studio Code (VS Code) is a free code editor that lets you write and manage your programming files.

1. Visit https://code.visualstudio.com/
2. Download the installer for your operating system.
3. Open the downloaded installer.
4. Follow the installation instructions.
5. Launch Visual Studio Code.

## ⚙️ Step 2: Install a C Compiler

A compiler converts your C source code into a program your computer can execute.

### Option A: Windows

One beginner-friendly option is **MSYS2**, which provides GCC for Windows.

1. Visit https://www.msys2.org/
2. Download and install MSYS2.
3. Open the **MSYS2 UCRT64** terminal from the Start menu.
4. Run this command to install the GCC compiler:

   ```bash
   pacman -S --needed mingw-w64-ucrt-x86_64-gcc
   ```

5. Follow any prompts to complete the installation.
6. Add the following folder to your Windows `Path` environment variable:

   ```text
   C:\msys64\ucrt64\bin
   ```

7. Close and reopen your terminal or VS Code.

Check that GCC is installed by running:

```bash
gcc --version
```

If a version number appears, GCC is available in your terminal.

### Option B: macOS

1. Open the Terminal application.
2. Run:

   ```bash
   xcode-select --install
   ```

3. Follow the installation instructions.
4. Check your compiler:

   ```bash
   clang --version
   ```

macOS provides Clang, which can compile C programs using commands similar to GCC.

### Option C: Linux

On Ubuntu or Debian, open a terminal and run:

```bash
sudo apt update
sudo apt install build-essential
```

Then check the compiler:

```bash
gcc --version
```

## 🧩 Step 3: Set Up VS Code for C

1. Open Visual Studio Code.
2. Select the Extensions icon on the left.
3. Search for **C/C++**.
4. Install the Microsoft C/C++ extension.
5. Create a folder for your project.
6. Open that folder in VS Code by selecting **File → Open Folder**.

The extension provides helpful features such as code highlighting, error assistance, and debugging support. It does not replace the compiler.

## 📝 Step 4: Create Your First C File

Now it is time to write your program!

1. In VS Code, open your project folder.
2. Create a new file.
3. Name it `main.c`.

The `.c` extension identifies the file as C source code.

4. Type the following code into the file:

   ```c
   #include <stdio.h>

   int main() {
       printf("I love GD!\n");
       printf("It's really great!");

       return 0;
   }
   ```

5. Save the file using **Ctrl + S** on Windows or **Command + S** on macOS.

Congratulations! You have created your first C source file.

## 🔍 Step 5: Understand the Code

### 1. The standard input/output library

```c
#include <stdio.h>
```

This includes the standard input/output library, which provides functions such as `printf()`.

### 2. The main function

```c
int main() {
```

The `main()` function is where a typical C program begins executing.

### 3. Displaying the first message

```c
printf("I love GD!\n");
```

The `printf()` function displays text on the screen. The `\n` moves the next output to a new line.

### 4. Displaying the second message

```c
printf("It's really great!");
```

This displays the second message. Because the first message ends with `\n`, the two messages appear on separate lines.

### 5. Ending the program

```c
return 0;
```

This indicates that the program has finished successfully.

### 6. Closing the main function

```c
}
```

The closing brace marks the end of the `main()` function.

## ▶️ Step 6: Compile Your Program

Open the VS Code terminal by selecting **Terminal → New Terminal**.

Make sure the terminal is in the folder containing `main.c`.

### Windows with GCC

Run:

```bash
gcc main.c -o main.exe
```

### macOS or Linux

Run:

```bash
gcc main.c -o main
```

If you are using Clang on macOS, you can use `clang` instead of `gcc`.

The compiler checks your source code and creates an executable program if compilation succeeds.

If you see an error, check your spelling, quotation marks, semicolons, and braces.

## 🚀 Step 7: Run Your Program

After compiling, execute the program.

### Windows

```powershell
.\main.exe
```

### macOS or Linux

```bash
./main
```

You should see this output:

```text
I love GD!
It's really great!
```

You have now successfully written, compiled, and run a C program!

## 🛠️ Step 8: Make Changes to Your Code

You can experiment by changing the messages inside the `printf()` functions.

For example:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    printf("I am learning C programming!");

    return 0;
}
```

Save the file, compile it again, and run the program to see the new output.

**Tip:** Every time you change the source code, compile it again before running the updated executable.

## 📂 Step 9: Organize Your Project

Your project folder can look like this:

```text
I-Love-GD/
├── main.c
└── README.md
```

- `main.c` contains your C source code.
- `README.md` explains what the project does and how to run it.

You can add more files as your project grows.

## 🌐 Step 10: Upload Your Project to GitHub

GitHub allows you to store your code online and share your programming projects.

1. Visit https://github.com/
2. Sign in or create an account.
3. Click the **New repository** option.
4. Name the repository `I-Love-GD`.
5. Add a short description, such as `My first C programming project`.
6. Choose whether the repository should be public or private.
7. Create the repository.

### Upload your files

You can upload the files through GitHub's website:

1. Open your new repository.
2. Select **Add file → Upload files**.
3. Upload `main.c` and `README.md`.
4. Add a commit message, such as `Add my first C program`.
5. Select **Commit changes**.

Your project files will now be stored in your GitHub repository.

## 📚 What I Learned

By completing this project, I practiced:

- Writing a C program from scratch.
- Using the `stdio.h` library.
- Printing text with `printf()`.
- Understanding the `main()` function.
- Using newline characters.
- Compiling source code.
- Running an executable program.
- Organizing files in a project folder.
- Sharing code on GitHub.

## 🔮 Future Improvements

In future versions, I could add:

- More messages using `printf()`.
- User input with `scanf()`.
- Variables to store information.
- Conditional statements.
- Loops and other programming exercises.

## 👨‍💻 Author

Created as a beginner C programming project to practice coding and learn the fundamentals of software development.

## 📄 License

This project is available for learning and educational purposes. You may use it as a starting point for your own beginner C programming projects.

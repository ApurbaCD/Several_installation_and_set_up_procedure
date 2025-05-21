# To Read more specificllly  -> https://code.visualstudio.com/docs/cpp/config-linux



# Using C++ on Linux in VS Code

## 1: Install Visual Studio Code.
## 2: Install the C++ extension for VS Code. You can install the C/C++ extension by searching for 'c++' in the Extensions view (Ctrl+Shift+X).
## 3: Ensure GCC is installed
###  First, check to see whether GCC is already installed. To verify whether it is, open a Terminal window and enter the following command:

```
gcc -v

```
### If GCC isn't installed, run the following command from the terminal window to update the Ubuntu package lists. An out-of-date Linux distribution can sometimes interfere with attempts to install new packages.
```
sudo apt-get update

```
### Next install the GNU compiler tools and the GDB debugger with this command:
```
sudo apt-get install build-essential gdb
```
### ( Create helloworld.cpp ) The code . command opens VS Code in the current working folder, which becomes your "workspace". As you go through the tutorial, you will create three files in a .vscode folder in the workspace:

    tasks.json (compiler build settings)
    launch.json (debugger settings)
    c_cpp_properties.json (compiler path and IntelliSense settings)

<!-- many things are not introduced -->

# Run helloworld.cpp

### 1: Open helloworld.cpp so that it is the active file.
### 2: Press the play button in the top right corner of the editor.
### 3: Choose g++ build and debug active file from the list of detected compilers on your system.(You'll only be asked to choose a compiler the first time you run helloworld.cpp. This compiler will be set as the "default" compiler in tasks.json file.)
### 4: After the build succeeds, your program's output will appear in the integrated Terminal.(The first time you run your program, the C++ extension creates tasks.json, which you'll find in your project's .vscode folder. tasks.json stores build configurations.

Your new tasks.json file should look similar to the JSON below:)
### **File and Directory Navigation 📁**

* pwd: print working directory. Shows you the full path of the directory you're currently in.  
* ls: list. Lists the files and directories in your current location. Use ls \-l for a detailed list (long format) and ls \-a to show hidden files.  
* cd: change directory. Used to navigate between directories.  
  * cd \[directory\_name\]: Moves you into the specified directory.  
  * cd ..: Moves you up one level to the parent directory.  
  * cd: Moves you to your home directory.  
* Which`:` command **locates an executable program** in your system's search path. It tells you the exact location (the full path) of the command that will run when you type its name in the terminal. 📍

| which python3/opt/homebrew/bin/python3 |
| :---- |

---

### **File and Directory Manipulation 📝**

* touch: Creates a new, empty file. For example, touch newfile.txt.  
* mkdir: make directory. Creates a new directory. For example, mkdir new\_folder.  
* cp: copy. Copies files and directories.  
  * cp \[source\] \[destination\]: Copies a file.  
  * cp \-r \[source\_dir\] \[destination\_dir\]: Recursively copies a directory and its contents.  
* mv: move. Moves or renames files and directories.  
  * mv \[old\_name\] \[new\_name\]: Renames a file or directory.  
  * mv \[source\] \[destination\]: Moves a file or directory.  
* rm: remove. Deletes files and directories.  
  * rm \[file\_name\]: Deletes a file.  
  * rm \-r \[directory\_name\]: Recursively deletes a directory and all its contents. Use with caution\!  
* truncate: Truncate a file to a specified size. The \-s option specifies the size, and 0 sets the file size to zero, effectively clearing its content. For example, truncate \-s 0 filename.txt.

---

### **Viewing and Editing Files 📖**

* cat: catenate. Displays the entire content of a file on the screen.  
* less: Displays file content one page at a time, allowing you to scroll. Press q to quit.  
* nano: A simple and user-friendly text editor. For example, nano my\_file.txt.

#### Nano-specific Commands:

* Paste:  
  * Windows: Use Ctrl \+ Shift \+ V or right-click.  
  * macOS: Use Cmd \+ V.  
  * Linux: Use Ctrl \+ Shift \+ V.  
  * Nano's internal paste: Use Ctrl \+ U after using Alt \+ 6 to copy within Nano.  
* Save: Press Ctrl \+ O ("Write Out") and then Enter to save the file.  
* Save and Exit: Press Ctrl \+ X. Nano will prompt you to save if you have unsaved changes. Press Y for "yes" and then Enter.  
* Remove All Content:  
  * Inside Nano: Press Alt \+ \\ to go to the beginning of the file, then Ctrl \+ 6 to set a mark, then press Alt \+ / to select all text, then Ctrl \+ K to cut the entire content, and finally Ctrl \+ O to save the now empty file.  
  * From the shell (outside Nano): Use the commands \> filename.txt or truncate \-s 0 filename.txt to quickly and permanently empty a file.

---

### **System Information and Help ℹ️**

* man: manual. Provides the manual page for a command, explaining its usage, options, and more. For example, man ls.  
* echo: Displays a line of text on the terminal. Useful for scripts. For example, echo "Hello, world\!".  
* clear: Clears the terminal screen.  
* exit: Closes the current terminal session.

---

### **User and Permissions 👨‍💻**

* sudo: super user do. Executes a command with administrative or root privileges.  
* whoami: Displays your current username.  
* passwd: Changes a user's password.

---

### **Process Management 🚦**

* ps: process status. Shows currently running processes.  
* top: Displays a real-time, dynamic view of running processes and system resource usage. Press q to quit.  
* kill: Terminates a process. You need the process ID (PID) from ps or top. For example, kill \[PID\].

---

### 

### **asciinema**

asciinema is a command-line tool that **records your terminal sessions** as lightweight, shareable text files instead of video. This allows viewers to copy and paste text directly from the recording. 🎬

#### **Core Commands**

* asciinema rec: Starts a new recording.  
* asciinema play \<filename\>: Plays back a locally saved recording in your terminal.  
* asciinema upload \<filename\>: Uploads a recording to asciinema.org to get a shareable link.

#### **How to Workflow**

1. **Install it**. On macOS, use brew install asciinema. On Debian/Ubuntu, use sudo apt install asciinema.  
2. **Start recording** by running asciinema rec. Perform your commands.  
3. **Stop recording** by typing exit or pressing **Ctrl+D**.  
4. **Press Enter** when prompted to instantly upload and get a shareable web link.

---

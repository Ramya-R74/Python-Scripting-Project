# My Python Automation Project

I built this project to sharpen my **Python scripting** skills and get hands-on experience with automating real-world developer workflows. By creating this tool, I learned how to manage file systems and trigger system-level tasks directly from my own code.

## What I Built
My script acts as a smart organizer. It scans through a messy `data` directory, picks out only the specific subdirectories related to my game projects, copies them into a clean destination folder while renaming them, and finally automates the compilation of the Go source code found inside each one.

## Key Skills I Applied
*   **Dynamic Inputs:** I used `sys.argv` to make my script flexible, allowing me to pass different source and target paths right from the command line.
*   **File System Mastery:** I practiced using `os.walk` to navigate through complex directories and `os.path.join` to ensure my code stays cross-platform.
*   **Efficient File Management:** I utilized `shutil` to handle the recursive copying and directory cleanup operations safely.
*   **Data Reporting:** I implemented a `metadata.json` generator to summarize the project results, giving me experience with JSON serialization and context managers.
*   **System Automation:** I bridged Python with my system shell using `subprocess.run` to automatically trigger `go build` commands, which was a huge highlight for me.

## How I Set It Up
1.  **Preparation:** I organized my workspace and ensured I had the Go compiler installed.
2.  **Scripting:** I wrote the logic to filter folders based on a "game" pattern and then executed the file system operations.
3.  **Refinement:** I added error handling and logical checks to ensure that the script only acts on valid directories containing `.go` files.

## Running the Project
Whenever I want to process my game files, I just run this command in my terminal:

`python get_game_data.py <source_directory> <target_directory>`

This project really bridged the gap between basic Python syntax and practical software engineering, and I feel much more confident in writing tools that save me time.

# Desktop Cleaner

Effortlessly organize files in a specific directory by tracking file types and moving them into designated folders.

## Setup
This project requires:
- **Python 3**
- **PIP**

Ensure your SSH keys are stored in GitHub if you're creating projects from this machine.

## How It Works
This script is designed to:
- Monitor a specific directory (e.g., desktop) for newly added files
- Automatically move the files to a designated location
- Run continuously in the background
- Organize files into categorized folders based on their types, with further organization by date. For example:
  - 2019
    - September
      - 9th
- Identify and handle all file types to determine new additions.

## Installation
1. Clone the project repository.
2. Navigate to the project directory.
3. **Optional**: Create a virtual environment:
   - `python3 -m venv venv`
   - Activate it with `source venv/bin/activate`, and deactivate with `deactivate`.
4. Install dependencies:
   - Ensure you have two folders: one for tracking (e.g., `oldDesktop`) and another for the destination (e.g., `newDesktop`). If you choose different folder names, update the script accordingly.
   - Install the required library using `pip install watchdog`.
   - Ensure the destination folder contains predefined categories (e.g., Media, Images, Videos, Programming). Missing folders will cause the script to fail.

## Usage
1. Run the script with: `python cleandesk.py`.
2. To test, move a file into the tracked folder and observe its relocation to the organized destination.

### MacOS Background Execution
To run the script in the background on MacOS:
1. Open `Automator.app`.
2. Create a new application.
3. Add the "Run Shell Script" action from the Library Utilities section.
4. Enter the command to execute the script.
5. Save the application and use it to automate the process.

This script simplifies file management, ensuring a clutter-free workspace.


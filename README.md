# Git Automation Project

This project automates the process of pushing text from a `.txt` file to a Git repository, committing it to a new branch with the commit message "Calculation Update", and scheduling this task to run at a specified time every day.

## Prerequisites

- Python 3.x
- Git
- `schedule` library (install using `pip install schedule` or 'pip install -r requirements.txt')

## Project Structure

. ├── automate_git.py ├── text_1.txt └── README.md


- `automate_git.py`: The main Python script that performs the automation.
- `text_1.txt`: The text file to be pushed to the Git repository.
- `README.md`: This README file.

## Installation

1. Clone the repository:

git clone https://github.com/yourusername/git-automation-project.git
cd git-automation-project

2. Install the required Python library:
pip install schedule
or
pip install -r requirements.txt

4. Usage
3.1 Update the automate_git.py script with the correct paths for your text file and Git repository:
    file_path = "path/to/your/file.txt"
    repo_path = "path/to/your/repo"
3.2 Run the script:
    python automate_git.py
    The script will run continuously and push the text from the .txt file to the Git repository every day at the specified time (e.g., 10:00 AM).

5. How It Works
  The script uses the schedule library to schedule the push_to_git function to run at a specified time every day.
  The push_to_git function performs the following tasks:
  Changes to the repository directory.
  Creates a new branch named calculation-update.
  Adds the specified file to the staging area.
  Commits the changes with the commit message "Calculation Update".
  Pushes the changes to the remote repository.

6. Contributing
  Contributions are welcome! Please feel free to submit a Pull Request.

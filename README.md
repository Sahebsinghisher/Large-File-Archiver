# Large-File-Archiver

archive_project.sh is a Bash script designed to automatically find and archive large files (over 20MB) within a specified directory. The script checks if the directory exists, creates an archive folder if it doesn't already exist, and compresses the identified files into .gz format before moving them to the archive folder. This script is ideal for managing disk space by archiving older or large files systematically.

Features-
->Checks if the base directory exists and handles the error if not.
->Creates an archive folder if it's not already present in the base directory.
->Finds files larger than 20MB within the specified directory depth.
->Compresses and moves the large files to the archive folder.
->Provides timestamped logs of the archiving process.
Usage-
->Clone the repository and navigate to the directory containing archive_project.sh.
->Update the BASE variable in the script to point to the directory you want to manage.
->Run the script using:
bash command-
$./archive_project.sh

Automation with Crontab-
To automate the archiving process, you can set up a cron job using crontab -e and specify the timing and script name. For example, to run the script every day at midnight, you can add the following line to your crontab:

To automate the script-
0 0 * * * /path/to/archive_project.sh
This will execute the script daily at 12:00 AM.

Requirements-
->A Linux environment with Bash.
->The gzip command should be available in the system.
->Sufficient permissions to read and write in the specified directory.

License-
This project is licensed under the MIT License - see the LICENSE file for details.

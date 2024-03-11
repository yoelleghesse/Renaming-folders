The Batch Rename Files in Directory script is a Python script that recursively iterates through a directory and renames all files within it based on the names of their parent folders. It utilizes the pathlib module to work with file paths and directories.

Clone the repo:

``git clone https://github.com/your-username/batch-rename-files.git``

Run the script:

``python batch_rename_files.py``

Features:

- Recursively iterates through a directory and its subdirectories.
- Renames all files within each subdirectory based on the names of their parent folders.
- Uses the pathlib module for handling file paths and directories in a platform-independent manner.

Config:

- Modify the root_dir variable to specify the directory where the files to be renamed are located.
- Ensure that the directory structure follows the pattern where each file's parent folder name will be used for renaming.


Ex., Suppose you have the following directory structure:

``files/
    ├── folder1/
    │   ├── file1.txt
    │   └── file2.txt
    ├── folder2/
    │   ├── file3.txt
    │   └── file4.txt
    └── folder3/
        ├── file5.txt
        └── file6.txt
``


After running the script, the files will be renamed as follows:

``files/
    ├── folder1/
    │   ├── folder1-file1.txt
    │   └── folder1-file2.txt
    ├── folder2/
    │   ├── folder2-file3.txt
    │   └── folder2-file4.txt
    └── folder3/
        ├── folder3-file5.txt
        └── folder3-file6.txt
``

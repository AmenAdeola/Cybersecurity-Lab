# File & directory management

Commands | Purpose | Example Result|
--------|---------|----------------|
cp | Copies a file or directory into a new location; the file will not be removed from the previous location | cp permissions.txt /home/analyst/logs: Copies the permissions.txt file from the user's current working directory to the logs directory
mkdir | Creates a new directory| mkdir network: Creates a new directory named network in the user's current working directory; mkdir /home/analyst/logs network:Creates a new directory named network in the logs directory; the full path is required when logs is not a subdirectory of the current directory
mv| Moves or rename a file or directory to a new location; the file is also removed from the previous location| mv permissions.txt /home/analyst/logs: Moves the permissions.txt file from the user's current working directory to the logs directory; mv permissions.txt perm.txt: Moves the permissions.txt file from the user's current working directory to the new file name perm.txt in the user's current working directory; this results in renaming the permissions.txt file as perm.txt
nano | Opens or creates a file in the nano command-line file editor| nano permissions.txt: Opens an existing permissions.txt file in the nano file editor, or creates the permissions.txt file in the nano file editor if it doesn't already exist in the current working directory
rm | Removes, or deletes, a file| rm permissions.txt: removes the permissions.txt file from the user's current working directory; rm home/analyst/reports/permissions.txt: Removes the permissions.txt file from from the reports directory; the full path is required if the user's current working directory is not reports
rmdir | Removes, or deletes, a directory; only removes directories if they are empty| rmdir network: Removes the empty network subdirectory of the user's current working directory from the file system; rmdir /home/analyst/logs/network: Removes the empty network directory from the file system; the full path is required when network is not a subdirectory of the current directory
touch|Creates a new empty file|touch permissions.txt: Creates a new file named permissions.txt in the user's current working directory; touch/home/analyst/reports/permissions.txt: Creates a new file named permissions.txt in the reports directory; the full path is required if the user wants to create permissions.txt in any directory other than the current working directory



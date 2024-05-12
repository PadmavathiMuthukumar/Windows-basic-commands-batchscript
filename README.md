# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript
# Developed by: PADMAVATHI.M
# Register number: 212223040141
# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/110b138d-8d42-4538-8601-324e87d4b2d3)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/1db40059-38fa-4591-bf61-3f15672ffc5a)


![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/beb6cd00-6578-4911-99db-8cb0c1d49463)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/d94338dc-a81a-4eee-a80a-fcdede389ffb)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/df5478d2-aee9-40bd-9847-641b80df1664)

![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/c2ecd6d7-344d-419b-9dec-f0e9304b896a)

Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/be3a11ff-25be-436c-9f27-0921bccd5487)
## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![image](https://github.com/PadmavathiMuthukumar/Windows-basic-commands-batchscript/assets/154965880/c8c4d90d-f1b2-4c0f-8a2f-f98d8273620b)

# RESULT:
The commands/batch files are executed successfully.


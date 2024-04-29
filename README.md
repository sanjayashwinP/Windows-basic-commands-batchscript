# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript     
DEVELOPED BY:SANJAY ASHWIN.P       
REG.NO:212223040181     
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

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/22e18ae3-b756-4425-b879-52551c9fdee0)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/95c71981-dbf5-45f9-b1de-b82e0f168f5c)

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/93cf768e-3b09-4f10-b99d-69764a31ee91)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/7fc686f7-fed5-44a6-a573-4e4bd3ea941f)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/05941f61-7777-4e12-a56f-0f620a592e1a)

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/0fa6835a-4df6-4c9c-b4f1-908e9ec20009)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/8cef4169-e646-4f96-acc1-25b763bc8c01)

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

![image](https://github.com/sanjayashwinP/Windows-basic-commands-batchscript/assets/147473265/8bf17e7f-dbcb-4ba9-9ffe-b474e3242e05)




# RESULT:
The commands/batch files are executed successfully.


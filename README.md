# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

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
```
mkdir %userprofile%\Desktop\MyLab
```
![329449798-398612b3-9655-420e-a9c9-f200a24d5232](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/8e5934b5-9037-4bc8-9b0a-bccc2d157090)

## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
![329451087-56ead55b-3ebc-457a-9b66-9e794536ea8d](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/2278bea0-9908-4666-8d15-72d7fc88127a)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![329449993-d1900a0b-4c3c-4770-bafa-39161e0a2c1c](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/15698a80-11d6-489f-9a8c-85c5c069775e)
![329450045-bffe5243-b728-440c-af14-be8e5105bab9](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/5e48a329-2c01-49d6-ae3a-b7882aaead60)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![329450216-ed4e8f45-9c2b-4c9a-9220-63bd3cfe0baa](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/1b9b52a0-1fe3-467f-9b24-63282f50f8aa)

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![329450372-a71f24b7-e9c4-40c6-a824-55f3466b4095](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/0d2474c9-82e6-4f69-9d74-248377fd24ea)
![329450418-6b368260-d83c-4bb4-bdb8-8fd0601a9dd7](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/085afd35-c579-4ca3-88a9-a29c1598c7ba)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![329450533-49dd374a-73a4-47f1-946f-86963b81a5b6](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/115665c1-1afc-4fcd-aa16-aa098fc0578c)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![329450771-e6f191cf-508d-4d3e-91da-9b9c27b9ab4c](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/4f4d328e-a76c-4db0-8337-3d8895b9cb13)




# RESULT:
The commands/batch files are executed successfully.


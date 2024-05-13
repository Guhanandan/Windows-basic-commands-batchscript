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

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```

![329658320-0d1c931c-0132-467e-a239-1a645505b196](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/5884aa47-0a97-4bd0-a67f-1b083749a81c)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![329659051-f2ae583f-91e3-49ac-bdcf-959749805451](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/11c3c540-573e-4f0e-83e1-b0782390d6bb)

```
type nul > MyFile.txt
```
![329659348-6a8337f0-c88f-4b81-a611-16e5f0bec7f7](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/9f9eb570-57aa-4cdf-9a12-8527c7d0b5ed)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```
![329659599-066144e3-43b8-4d7c-bf48-8a03d75d6c7e](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/a1e3371e-00f3-43e7-973a-cdc5372286cd)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup
```
![329659806-7a228e90-8940-43be-8231-4766db062bb7](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/c5c4a187-f273-4bea-94c3-0f0035284fe0)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![329659991-e045c571-5703-455a-8d32-9aa6b2a2afde](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/ca0caf7f-637e-4249-a96d-77d2c0785160)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![329660496-6b0dcb2a-0b98-4712-ac5a-4d558ca37037](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/0248bc54-6b04-451c-b141-52df5029c4ab)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


## COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
## OUTPUT
![329660834-0594a6df-84d8-4328-a347-5e6ca215a41c](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/42ab92aa-6068-48fb-b536-151983e99875)

## COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![329661256-27953f04-f5d1-4b1f-a369-60b6cb1d90e1](https://github.com/Guhanandan/Windows-basic-commands-batchscript/assets/100425381/9e15ea9e-f8a1-413c-9ebb-ebc9a447b367)



# RESULT:
The commands/batch files are executed successfully.


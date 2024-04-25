# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

### Developed by: SURIYA M

### Reg no      : 212223110055

## AIM:
To execute Windows basic commands and batch scripting

## DESIGN STEPS:

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

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/0734ccbd-f714-46af-be2f-b3a57b460f35)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/f3ecc818-3096-4141-b2fb-20a5f9556f13)

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/b3a710eb-3a65-4070-858e-8af90b42f1dd)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/8a3d2552-83b0-4ad6-9497-75543a638008)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/51f6a1ba-722a-4376-97c8-c0700d26018a)

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/0614aa49-9651-49d3-8734-165e7549f99d)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/cc4e5f66-05d4-4160-96ed-866e257ce0e5)

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

![image](https://github.com/Suriya-MD/Windows-basic-commands-batchscript/assets/147120571/1a5af381-5380-4191-b910-6f9c432c6706)

## RESULT:
The commands/batch files are executed successfully.



**Ex:08**
# Windows-basic-commands-batchscript
**DATE:** 
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
**NAME : SUBHASHINI.B**  
**REGISTER NUMBER: 212223040211**  
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot from 2024-04-30 11-01-47](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/f1f83410-e659-40ff-bee3-e079d93c7736)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.



## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```

![Screenshot from 2024-04-30 11-02-07](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/4de1b4bd-f842-485a-bf0d-90def6eaf1e9)
![Screenshot from 2024-04-30 11-01-57](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/60ef83ad-950a-4bf7-ae70-7ccd4fae7aa7)





## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
dir %userprofile%\Desktop\MyLab
```

![Screenshot from 2024-04-30 11-02-20](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/a28afee5-4fc8-4720-a29b-ae4c9819f177)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot from 2024-04-30 11-02-33](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/ad0e4f9e-575b-48f5-95fe-7df3f52b5857)
![Screenshot from 2024-04-30 11-02-46](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/fc1a73ef-f263-4896-9465-239e1420b390)



## COMMAND AND OUTPUT

```
mv Myfile.txt %userprofile%\Documents
```

![Screenshot from 2024-04-30 11-02-51](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/0fe73689-4d9b-4494-8ce8-d940fc9b9606)

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


![Screenshot from 2024-04-30 11-03-00](https://github.com/shivsujan/Windows-basic-commands-batchscript/assets/145633245/f8257a6d-6fa4-4e1a-bc73-063fad3c5508)



# RESULT:
The commands/batch files are executed successfully.


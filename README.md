# EX08 Windows-basic-commands-batchscript

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

**NAME : SUBHASHINI.B**  
**REGISTER NUMBER: 212223040211**  


# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/6cdd8e0d-bb77-4a26-a6dc-7c9d5d47cc85)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-13 095506](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/ea2d3bda-7b88-4601-9f61-013d3011d914)


```
type nul > MyFile.txt
```

![image](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/8d3788e2-8862-4513-9180-ee31af9f5786)




List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-13 095752](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/ea9138fe-d025-4495-bb9a-baaf8c0f17bb)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
```
![Screenshot 2024-05-13 095824](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/4edbe7ad-e79c-43ba-a84e-ca1524a55ae0)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-05-13 095855](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/e4e6964b-4c48-42bb-aa29-35e86ffcd865)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![Screenshot 2024-05-13 095925](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/7e9b87a3-fe8e-40dd-aba0-eb3136e1cc32)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.




## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```


## OUTPUT:
![image](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/79a7e770-0642-451f-9496-eccad6a24cf5)

## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT:
![Screenshot 2024-05-13 100045](https://github.com/subha-shinibalasubramanian/Windows-basic-commands-batchscript/assets/164154478/59c20c41-fd81-47ca-a764-85643f574ac5)

# RESULT:
The commands/batch files are executed successfully.


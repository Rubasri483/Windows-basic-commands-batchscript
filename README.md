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

<img width="692" height="102" alt="image" src="https://github.com/user-attachments/assets/c8be2f35-834c-4cdb-8b01-23e62b860205" />



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

<img width="592" height="66" alt="image" src="https://github.com/user-attachments/assets/426a2607-cb4e-4785-b310-5e18c977546b" />



Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

<img width="750" height="378" alt="image" src="https://github.com/user-attachments/assets/252517a0-92c9-4676-b7fb-d6114d5b74b9" />


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

<img width="700" height="108" alt="image" src="https://github.com/user-attachments/assets/47feb30a-4073-4151-a21b-e327f5dc1ce7" />


Copy the file hello.txt into the file hello1.txt

## COMMAND AND OUTPUT

<img width="592" height="143" alt="image" src="https://github.com/user-attachments/assets/4168abc2-b4e0-47ba-b906-65cffbf99ef6" />

List out the file hello1.txt in the current directory

## COMMAND AND OUTPUT

<img width="661" height="195" alt="image" src="https://github.com/user-attachments/assets/46e8cbdf-fa50-4900-87e8-ee87ebc7fc1f" />


List out all the associated file extensions

## COMMAND AND OUTPUT

<img width="707" height="488" alt="image" src="https://github.com/user-attachments/assets/a6a0f387-9126-434a-88d0-d9cb276332f5" />


Compare the file hello.txt and rose.txt

## COMMAND AND OUTPUT

<img width="668" height="206" alt="image" src="https://github.com/user-attachments/assets/0adb0318-f0ea-4d4b-8c4d-068acfe99bc5" />


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## BATCH PROGRAM
```
@echo off
set name=John
echo Hello, %name%
pause
```

<img width="761" height="380" alt="image" src="https://github.com/user-attachments/assets/adc89744-0ed2-4b9b-8ac5-de6f7bebf98c" />



## OUTPUT

![alt text](op10.png)


2.Create a batch file on the desktop that checks whether a user-input number is odd or not. The script should: Prompt the user to enter a number. Calculate the remainder when the number is divided by 2. Display whether the number is odd or not. Ask the user if they want to check another number. Repeat the process if the user enters Y, and exit with a thank-you message if the user enters N. Handle invalid inputs for the continuation prompt (Y/N) gracefully.

## BATCH PROGRAM

```
@echo off
:loop
set /p num=Enter a number: 
set /a rem=%num% %% 2

if %rem%==0 (
    echo %num% is Even
) else (
    echo %num% is Odd
)

:ask
set /p ans=Do you want to check another number? (Y/N): 
if /I "%ans%"=="Y" goto loop
if /I "%ans%"=="N" goto end
echo Invalid input. Please enter Y or N.
goto ask

:end
echo Thank you!
pause
```

## OUTPUT

![alt text](op11.png)

3.Write a batch file that uses a FOR loop to iterate over a sequence of numbers (1 to 5) and displays each number with the label Number:. The output should pause at the end.

## BATCH PROGRAM

```
@echo off
for /L %%i in (1,1,5) do (
    echo Number: %%i
)
pause
```

## OUTPUT

![alt text](op12.png)

4.Write a batch script to check whether a file named sample.txt exists in the current directory. If the file exists, display the message sample.txt exists. Otherwise, display sample.txt does not exist. Pause the script at the end to view the result.

Instructions: Use the IF EXIST conditional statement. Make sure the script works for files located in the same directory as the batch file. Use pause to keep the command window open after displaying the message. Expected Output (if the file exists):

## BATCH PROGRAM

```
@echo off
if exist sample.txt (
    echo sample.txt exists.
) else (
    echo sample.txt does not exist.
)
pause
```

## OUTPUT

![alt text](op13.png)

5.Write a batch script that displays a simple menu with three options: Say Hello – Displays the message Hello, World! Create a File – Creates a file named newfile.txt with the content This is a new file Exit – Exits the script with a goodbye message The script should repeatedly display the menu until the user chooses to exit. Use goto statements to handle menu navigation

## BATCH PROGRAM

```
@echo off
:menu
cls
echo 1. Say Hello
echo 2. Create a File
echo 3. Exit
set /p choice=Choose an option (1-3): 

if "%choice%"=="1" goto hello
if "%choice%"=="2" goto create
if "%choice%"=="3" goto exit
echo Invalid choice.
pause
goto menu

:hello
echo Hello, World!
pause
goto menu

:create
echo This is a new file > newfile.txt
echo File newfile.txt created.
pause
goto menu

:exit
echo Goodbye!
pause
exit
```

## OUTPUT

![alt text](op14.png)

# RESULT:
The commands/batch files are executed successfully.


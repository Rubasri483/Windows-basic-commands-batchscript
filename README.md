# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

#### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

#### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
#### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
### Exercise 1: Basic Directory and File Operations

Create a directory named "my-folder"
### COMMAND AND OUTPUT
<img width="606" height="223" alt="image" src="https://github.com/user-attachments/assets/748e6b9a-5b6e-4f43-b392-09fd0565b347" />


Remove the directory "my-folder"
### COMMAND AND OUTPUT

<img width="842" height="371" alt="image" src="https://github.com/user-attachments/assets/339bde79-e0e1-44f2-a2bd-038237af6fa5" />


Create the file Rose.txt
### COMMAND AND OUTPUT
<img width="828" height="352" alt="image" src="https://github.com/user-attachments/assets/c9298052-c5ee-426a-826a-34329257a959" />


Create the file hello.txt using echo and redirection
### COMMAND AND OUTPUT

<img width="960" height="121" alt="image" src="https://github.com/user-attachments/assets/b5efa2f2-d003-4e7c-961e-5739f7f6e535" />


Copy the file hello.txt into the file hello1.txt
### COMMAND AND OUTPUT
<img width="892" height="143" alt="image" src="https://github.com/user-attachments/assets/e69e2793-362c-4bcc-800a-b066d595ecba" />


Remove the file hello1.txt
### COMMAND AND OUTPUT

<img width="782" height="221" alt="image" src="https://github.com/user-attachments/assets/de4bf3e1-b0c4-4b95-ab7d-9cb9790a0526" />


List out the file hello1.txt in the current directory
### COMMAND AND OUTPUT
<img width="757" height="1059" alt="image" src="https://github.com/user-attachments/assets/76739fa0-5346-4bea-bf70-f753b49c1b60" />



List out all the associated file extensions 
### COMMAND AND OUTPUT
<img width="863" height="1106" alt="image" src="https://github.com/user-attachments/assets/350702db-c9d8-42b9-928d-c4e8c691cd3d" />


Compare the file hello.txt and rose.txt
### COMMAND AND OUTPUT
<img width="826" height="188" alt="image" src="https://github.com/user-attachments/assets/525e8702-09c3-4ba1-9217-948d0164ecac" />


## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".

### OUTPUT

<img width="697" height="89" alt="image" src="https://github.com/user-attachments/assets/8984aca1-330f-41b4-81cd-ac15bf7914f4" />



Create a batch file  on the desktop that checks whether a user-input number is odd or not. The script should:
Prompt the user to enter a number.
Calculate the remainder when the number is divided by 2.
Display whether the number is odd or not.
Ask the user if they want to check another number.
Repeat the process if the user enters Y, and exit with a thank-you message if the user enters N.
Handle invalid inputs for the continuation prompt (Y/N) gracefully.

### OUTPUT

<img width="693" height="260" alt="image" src="https://github.com/user-attachments/assets/0b1ec684-0daf-47cb-a06d-31225fcc5368" />



Write a batch file that uses a FOR loop to iterate over a sequence of numbers (1 to 5) and displays each number with the label Number:. The output should pause at the end.

### OUTPUT
<img width="715" height="209" alt="image" src="https://github.com/user-attachments/assets/209322ea-5b1a-4eee-936a-06022fd9cf3c" />



Write a batch script to check whether a file named sample.txt exists in the current directory. If the file exists, display the message sample.txt exists. Otherwise, display sample.txt does not exist. Pause the script at the end to view the result.

Instructions:
Use the IF EXIST conditional statement.
Make sure the script works for files located in the same directory as the batch file.
Use pause to keep the command window open after displaying the message.
Expected Output (if the file exists):

### OUTPUT

<img width="696" height="111" alt="image" src="https://github.com/user-attachments/assets/b095b05a-a0b3-4de4-9782-6cd5a13c2433" />



Write a batch script that displays a simple menu with three options:
Say Hello – Displays the message Hello, World!
Create a File – Creates a file named newfile.txt with the content This is a new file
Exit – Exits the script with a goodbye message
The script should repeatedly display the menu until the user chooses to exit. Use goto statements to handle menu navigation.


### OUTPUT

<img width="753" height="442" alt="image" src="https://github.com/user-attachments/assets/6a1cca41-3938-40cf-adea-16f570e30e5b" />



# RESULT:
The commands/batch files are executed successfully.

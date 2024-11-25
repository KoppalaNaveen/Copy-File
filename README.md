# Copy-File
## AIM:
To write a python program for copying the contents from one file to another file.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import the necessary library to handle file uploads.
### Step 2: 
Create a function called copy_file that takes two parameters: source and destination.
### Step 3: 
Inside the function, open the source file in read mode and read its contents.
### Step 4:  
Open the destination file in write mode and write the contents read from the source file into it.
### Step 5: 
Print a success message indicating that the contents have been copied.
### Step 6: 
Handle any errors that may occur, such as file not found or other exceptions.
## PROGRAM:
```
def copy_file(source, destination):
    try:
        with open(source, 'r') as src_file:
            content = src_file.read()
        with open(destination, 'w') as dest_file:
            dest_file.write(content)
        print(f"Contents copied from {source} to {destination}.")
    except FileNotFoundError:
        print(f"Error: The file {source} does not exist.")
    except Exception as e:
        print(f"An error occurred: {e}")

source_file = 'source.txt'  
destination_file = 'destination.txt'

copy_file(source_file, destination_file)

```
### OUTPUT:

![image](https://github.com/user-attachments/assets/1c5813f6-d514-4075-a9de-2e8163c96573)

## RESULT:
Thus the program is written to copy the contents from one file to another file.

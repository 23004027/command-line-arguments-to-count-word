# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
# Step 1:
Import the sys module.

# Step 2:
Define a function get_word_count(file_path) to calculate the word count in the file.

# Step 3:
Check if the script is being run as the main program

# Step 4:
Check if the correct number of command-line arguments (i.e., 2) is provided.

# Step 5:
Get the file path from the command-line argument

# Step 6:
Print the word count if it is not None.

# Step 7:
End the program

## PROGRAM:
```python
Program for getting the word count using command line arguments.
Developed by:VIGNESH.V 
Register number: 23004027
import sys
def get_word_count(file_path):
    try:
        with open(file_path, 'r') as file:
            content = file.read()
            word_count = len(content.split())
            return word_count
    except FileNotFoundError:
        print(f"Error: File '{file_path}' not found.")
        return None
if name == "main":
    if len(sys.argv) != 2:
        print("Usage: python word_count.py <file_path>")
        sys.exit(1)
    file_path = sys.argv[1]
    word_count = get_word_count(file_path)
    if word_count is not None:
        print(f"Word count in '{file_path}': {word_count}")
```
### OUTPUT:
![Screenshot 2024-01-02 165447](https://github.com/23004027/command-line-arguments-to-count-word/assets/138956447/a14c6ea8-c510-47a6-820e-c8e31737135d)
![WhatsApp Image 2024-01-02 at 17 17 03_1f650225](https://github.com/23004027/command-line-arguments-to-count-word/assets/138956447/37d08fd5-a219-4b6a-83b1-8aed7ac3325a)
![WhatsApp Image 2024-01-02 at 17 17 05_6c5002f4](https://github.com/23004027/command-line-arguments-to-count-word/assets/138956447/260a94f5-9e65-45d2-97bd-8d4042376420)
![WhatsApp Image 2024-01-02 at 17 17 06_498d8699](https://github.com/23004027/command-line-arguments-to-count-word/assets/138956447/e393075f-5cc6-4808-8f42-12ef222b57e9)



## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.

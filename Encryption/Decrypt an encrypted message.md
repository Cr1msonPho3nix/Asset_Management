# Scenario
In this scenario, all of the files in your home directory have been encrypted. You’ll need to use Linux commands to break the Caesar cipher and decrypt the files so that you can read the hidden messages they contain.

## 1. Read the contents of a file
- In this task, you need to explore the contents of your home directory and read the contents of a file to get further instructions. The README.txt file contains an important message with instructions you need to follow.
![Check_readme_message]()

## 2. Find a hidden file
- In this task, you need to find a hidden file in your home directory and decrypt the Caesar cipher it contains. This task will enable you to complete the next task.
- This cipher can be solved by shifting each alphabet character to the left or right by a fixed number of spaces. In this example, the shift is three letters to the left. Thus "d" stands for "a", and "e" stands for "b". [tr "d-za-cD-ZA-C" "a-zA-Z"]
![Decrypting_caesar]()

## 3. Decrypt a file
- In this task you need to use the command revealed in .leftshift3 to decrypt a file and recover your data so you can read the message it contains. Use the information on the text previously decrypted.
![Decrypting_Q1.files]()
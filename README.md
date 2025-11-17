# Count the Words Thread

## Objectives
This project aims to demonstrate the use of threading in C to read user input and count the number of words in that input efficiently.

## Problem
Create a program that utilizes a separate thread to handle user input. The thread will read lines of text until an empty line is entered and count the words in each line of text provided.

## Implementation
- Create a function **count_words** that takes a string input and counts the number of words present in it. It identifies words by checking for **spaces**, **newline characters**, or **tab characters**.

- Create a **count_words_thread** that prompts the user for input and reads lines until an empty line is submitted. For each line read, it calls the **count_words** function to count the words.

- In the Main method, create a thread that runs the **count_words_thread** function. It then waits for the thread to finish before displaying the total word count.

## Test case

Run the program
```
Enter text (press Enter to submit):
```
Write the following text
```
Enter text (press Enter to submit):
Thread management is easy.
```
Press **Enter**
```
Enter text (press Enter to submit):
Thread management is easy.
Number of words: 4
```
Write another text
```
Enter text (press Enter to submit):
Thread management is easy.
Number of words: 4
Every process has at least one thread to get executed. 
```
Press **Enter**
```
Enter text (press Enter to submit):
Thread management is easy.
Number of words: 4
Every process has at least one thread to get executed.
Number of words: 14
```
To exit and terminate the program, enter a new empty line and press **Enter**
```
Thread management is easy.
Number of words: 4
Every process has at least one thread to get executed.
Number of words: 14

Number of words: 14
Input finished.
```


## Submission 
- Fork the project and add your code to it.
- Successfully running the test case.
- Submit a pull request when you complete the project.
- Create an issue with your questions if you face any trouble solving the project.

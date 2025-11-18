# Count the Words Thread

## Objectives
This project aims to demonstrate the use of threading in C to efficiently read user input and count the number of words in that input.

## Problem
Create a program that utilizes a separate thread to handle user input. The thread will read lines of text until an empty line is entered and count the words in each line of text provided.

## Implementation

- Create a function `void *count_words_thread(void *arg)` that will be responsible for reading input lines and counting how many words are in the input, until the **Enter** key is clicked. 


In the Main method 
- Prompt the user to enter an input by printing the message **Enter text (press Enter to submit):**.
- Create a thread that runs the `count_words_thread` function. 
- It then waits for the thread to finish before displaying the total word count.


> [!TIP]
> Words are identified by checking for **spaces**, **newline characters**, or **tab characters**.


```C

#include <stdio.h>
#include <pthread.h>

#define MAX_INPUT_SIZE 1024
int count = 0;

void *count_words_thread(void *arg) {
    char input[MAX_INPUT_SIZE];

    while (1) {

        // Read a line of input
        if (fgets(input, MAX_INPUT_SIZE, stdin) != NULL) {

            // add your code here 

 }

    return NULL;
 }


int main() {

    // add your code here

    return 0;
}

```

## Test case

Run the program
```
Enter text (press Enter to submit):
```
Write the following text
```
Enter text (press Enter to submit):
Every process has at least one thread to get executed.
```
Press **Enter**
```
Enter text (press Enter to submit):
Every process has at least one thread to get executed.
Number of words: 10
Exiting...
```




## Submission 
- Fork the project and add your code to it.
- Successfully running the test case.
- Submit a pull request when you complete the project.
- Create an issue with your questions if you face any trouble solving the project.

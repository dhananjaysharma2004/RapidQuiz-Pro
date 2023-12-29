#RapidQuiz Pro

## Exercise Overview

RapidQuiz Pro is a two-part exercise designed to create a quiz game application in Go. The goal is to read quiz questions from a CSV file and engage users by providing immediate feedback on their answers.

## Part 1: Quiz Game

### Description

Create a program that reads quiz questions from a CSV file, allowing users to answer and tracking their performance. The CSV file format consists of pairs, where the first column represents a question, and the second column is the answer.

### CSV Format Example

```
5+5,10
7+3,10
1+1,2
8+3,11
1+2,3
8+6,14
3+1,4
1+4,5
5+1,6
2+3,5
3+3,6
2+4,6
5+2,7
```

## Features

    Default CSV file: problems.csv
    User-customizable filename via a flag
    Continuous presentation of questions regardless of the correctness of the previous answer
    Output total number of correct and total questions at the end

### Note

CSV files may contain questions with commas.

## Part 2: Timer Integration

### Description

Extend the program to include a timer. The default time limit is 30 seconds, but users can customize it via a flag. The quiz should terminate when the time limit is exceeded, even if the user hasn't answered the last question.

### Features

    Timer functionality with default limit (30 seconds)
    Customizable time limit via a flag
    Users prompted to start the quiz by pressing enter
    Questions displayed one at a time until the user answers
    Output total number of correct and total questions at the end, considering invalid and unanswered questions

### Implementation Notes

    Utilize the CSV package in Go for parsing.
    Encourage exploration of Go's timer functionality.

### Usage

Clone the Repository

````bash

git clone https://github.com/your-username/RapidQuiz-Pro.git ```

Run the Program

Follow the instructions in the exercise details to implement and test the functionality.
Example

```bash

./rapidquiz -file=myquiz.csv -time=45

````

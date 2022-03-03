# Requirements

## Introduction

The project is titled as **Book Cricket Game** and developed using C language. Book Cricket is an indoor game which can be played by kids with a book.This game is made for two players. The two players will have to decide who is going to guess the toss. After winning the toss, the player has to select whether he has to bat/bowl first. The player who is going to bat first, need to hold the book. He has to randomly open the pages of the book and look for the last digit of that page number which is nothing but the runs obtained in that particular ball. If the last digit is 7/8/9, then it will be considered as a dot ball. The obtained score will be added to the batsman's score everytime. The batsman will be out if the number is 0. Then, the second player has to play with the book in the same process.


### Advantages

 - Improved engagement with the gamers
 - Easy and faster access 
 - Better, longer-lasting customer relationships
 - Increased productivity with relaxation
 - No need of more memory for storage 
 - Random values generation makes our game more interesting.
 
 ### Disadvantages
 - Only two players can play this game
 - Leaderboard needs to be implemented
 - Cannot store the previous game statistics.
 
## Cost and Features
 - Complexity 
 - Random Function values generation
 - Finding the sum of the players score individually

## FLOW CHART Diagram
![FLOWCHART Diagram](https://github.com/naresh9908/M1_IndoorGame_BookCricket/blob/main/5_RelatedImageslink/flowchart.png)

##  Defining Goal
 ![Defining Goal](https://github.com/naresh9908/M1_IndoorGame_BookCricket/blob/main/5_RelatedImageslink/Cricket%20game.png)

- The two players will have to decide the number of batsman.
- Toss a coin and decide who is going to bat first.
 - The player decided to bat will hold the book with him.
- He has to randomly open the book and look for the page number.
- The player should always look for the side of book which has even numbers on it.
- In the opened page, look for the even number and take note of the last unit in that number. For Example: If the opened page is 154, then the last unit is 4 so the score is 4. So the possible scores are 2, 4, 6, 8 and 0.
2, 4 and 6 score will be added to the batsman score as such and 8 will be a dot ball or counted as a single, it is decided at the beginning of the game when the decide on the number of bats man . 0 score means the batsman is out.

- Close the book and open it again.

- Note the score for that again.

- The innings will go on until all the batsmen is out.

- The total score of the first player is noted and then the second player takes over the Book and continues to play.

At the end who ever has the bigger score is the Winner  
## SWOT Analysis
 
# 4 W's and 1 H

## Who
Every person with electrnic devices need games now a days.

## What
A book cricket game where two players can play with each other almost like real cricket.

## When

Due to the pandemic sitations, noone can go out and play cricket, so they can play this book cricket instead.

## Where

It can be played by everyone and everywhere irrespective of their age. 

## How

This application was developed in C language to avoid the complexity and to keep it simple. 


# Detail Requirements

## High Level Requirements
| ID | Description | Status |
|--|--|--|
| HR01 |Main Menu  | Implemented |
| HR02 | Can be played by 2 players | Implemented |
| HR03 | Toss |  Implemented |
| HR04 | Batting/Bowling |  Implemented |
| HR05 | Graphical User Interface | Future |


## Low Level Requirements 

| ID | Description | HR ID | Status |
|--|--|--|--|
| LR01 |Main menu should consist 4 options asking for 1.Limited Overs 2.Play Until Out 3.Instructions For the Game 4.Quit  | HR01| Implemented |
| LR02 | Reading the names of the two players and asking for the selection of head/tail while tossing the coin. | HR02| Implemented |
 LR03 | Implementing a function which takes the users according to the toss for the next steps which are batting/bowling. | HR03| Implemented |
| LR04 | If user searches for an invalid key "Invalid Input" message should be displayed | HR03| Implemented |
| LR05 |Implementing a fnction named batting which returns the total sum of the score of the two players. | HR04| Implemented |
| LR06 |A clean graphical user interface with all required buttons for ease of use  | HR05| Future |

# M1_Tic-Tac-Toe-game
# REQUIREMENTS
## Introduction
This report is an introduction to the �Tic Tac Toe Game� in C programming.
Anybody who doesn't know the basics of Tic Tac Toe in C,will certainly be able to understand and gain the great knowledge from this project.
The core theme of the report focuses on the development of Tic Tac Toe Game using C language.
### Advantages
The game of tic-tac-toe is a game of predictability.
The moves that are believed to be important are highly predictable.
This also makes it a game of opposites in a way, because this goes against the definition of an �important move"
We can also have brain wash to our capability of thinking and have fresh mind.
#### Disadvantages
this tic tac toc in c language is pretty much easy but takes time instead we can have simplicity of codes but takes time
so time taking for implementation
can perform directly on papar instaed of this.

# Architecture

1. Play occurs on a 3 by 3 grid of 9 empty squares.
2. Two players alternate marking empty squares, the first player marking "X"s and the second player marking "O"s.
3. If one player places three of the same marks in a row, that player wins.
4. If the spaces are all filled and there is no winner, the game ends in a draw
![1](https://user-images.githubusercontent.com/99128901/153709336-c22546b4-cfad-4371-96aa-2557b25bd203.jpg)

# Flowchart

# Implementation
#include <stdio.h>
#include <conio.h>

char square[10] = { 'o', '1', '2', '3', '4', '5', '6', '7', '8', '9' };

int checkwin();
void board();

int main()
{
    int player = 1, i, choice;

    char mark;
    do
    {
        board();
        player = (player % 2) ? 1 : 2;

        printf("Player %d, enter a number:  ", player);
        scanf("%d", &choice);

        mark = (player == 1) ? 'X' : 'O';

        if (choice == 1 && square[1] == '1')
            square[1] = mark;
            
        else if (choice == 2 && square[2] == '2')
            square[2] = mark;
            
        else if (choice == 3 && square[3] == '3')
            square[3] = mark;
            
        else if (choice == 4 && square[4] == '4')
            square[4] = mark;
            
        else if (choice == 5 && square[5] == '5')
            square[5] = mark;
            
        else if (choice == 6 && square[6] == '6')
            square[6] = mark;
            
        else if (choice == 7 && square[7] == '7')
            square[7] = mark;
            
        else if (choice == 8 && square[8] == '8')
            square[8] = mark;
            
        else if (choice == 9 && square[9] == '9')
            square[9] = mark;
            
        else
        {
            printf("Invalid move ");

            player--;
            getch();
        }
        i = checkwin();

        player++;
    }while (i ==  - 1);
    
    board();
    
    if (i == 1)
        printf("==>\aPlayer %d win ", --player);
    else
        printf("==>\aGame draw");

    getch();

    return 0;
}

/*********************************************

FUNCTION TO RETURN GAME STATUS
1 FOR GAME IS OVER WITH RESULT
-1 FOR GAME IS IN PROGRESS
O GAME IS OVER AND NO RESULT
 **********************************************/

int checkwin()
{
    if (square[1] == square[2] && square[2] == square[3])
        return 1;
        
    else if (square[4] == square[5] && square[5] == square[6])
        return 1;
        
    else if (square[7] == square[8] && square[8] == square[9])
        return 1;
        
    else if (square[1] == square[4] && square[4] == square[7])
        return 1;
        
    else if (square[2] == square[5] && square[5] == square[8])
        return 1;
        
    else if (square[3] == square[6] && square[6] == square[9])
        return 1;
        
    else if (square[1] == square[5] && square[5] == square[9])
        return 1;
        
    else if (square[3] == square[5] && square[5] == square[7])
        return 1;
        
    else if (square[1] != '1' && square[2] != '2' && square[3] != '3' &&
        square[4] != '4' && square[5] != '5' && square[6] != '6' && square[7] 
        != '7' && square[8] != '8' && square[9] != '9')

        return 0;
    else
        return  - 1;
}


/*******************************************************************
FUNCTION TO DRAW BOARD OF TIC TAC TOE WITH PLAYERS MARK
 ********************************************************************/


void board()
{
    system("clear");
    printf("\n\n\tTic Tac Toe\n\n");

    printf("Player 1 (X)  -  Player 2 (O)\n\n\n");


    printf("     |     |     \n");
    printf("  %c  |  %c  |  %c \n", square[1], square[2], square[3]);

    printf("_____|_____|_____\n");
    printf("     |     |     \n");

    printf("  %c  |  %c  |  %c \n", square[4], square[5], square[6]);

    printf("_____|_____|_____\n");
    printf("     |     |     \n");

    printf("  %c  |  %c  |  %c \n", square[7], square[8], square[9]);

    printf("     |     |     \n\n");
}

/*******************************************************************
END *******************************************************************/



# Output
![Screenshot (47)](https://user-images.githubusercontent.com/99128901/153711440-70986d51-442b-406a-801a-54c0ee518ae5.png)
![Screenshot (49)](https://user-images.githubusercontent.com/99128901/153711859-f526f1fa-ffb1-4041-af94-41e8d61b0130.png)


# Conclusion
The “Tic Tac Toe Game” is most familiar among all the age groups.Intelligence can be a property of any purpose-driven decision maker.
This basic idea has been suggested many times. An algorithm of playing Tic Tac Toe has been a great play.


# References
Google Wikipedia.
https://www.onlinegdb.com/online_c_compiler.
https://www.youtube.com/watch?v=3mrfOqjy9R8


# Acknowlegement
This mini project is for the sake of understating things and implementating.
I have made repository with learning through youtube which made me feel efficient way.
As i gone to massive clumsyness, but though things got settle after learning



# Simulator-to-WordScapes-on-Play-Store

Introduction:

—  In this project we will create the console-based simulator of the wordscapes games, where the user is given some letters and the user 
    has to guess the words from    those letters.

—  This game is designed for only 5 levels.

—  At each level the user will be given some letters and the user has to guess 3 words to move to the next level.

—  If the user guesses the wrong word at any chance, the user will lose one live point and will be asked to give another word.

—  The user will get 5 lives which means the user can make 5 wrong guesses.

—  After 5 wrong guesses the game will automatically get over and the user will get the final score.

—  But if the user makes correct 3 guesses, they will move to the next level.

—  At the end of each level the user will be asked if the user wants to continue or not.

—  If the user selects yes, the game will continue but if the user selects no then the game will stop at that level and the final score 
    will be displayed. 


Explanation:

—  In the program, first we have declared the letters and words, using these letters that we will form the words.

—  At each level the user will be given one set of letters and then the code will match each input of the user with the pre-defined set 
    of the word based on those letters.

—  We are using a list of lists for words named as words and another list of lists  for letters named as letters.

—  We have declared an integer variable named lives to control the number of the lives the user will have. The value of this variable 
    will be decremented if the user makes a wrong guess. We have initialized it to 5.

—  We have declared  an integer variable named level to control the level that the user is playing, we have initialized it to 0 as that 
    will be the index number for the first set of letters and words.

—  We have declared an integer variable named score for maintaining the score of the users. We have initialized it to 0 and this 
    variable value will be incremented for every correct guess made by the user.

—  Next, we have created a while loop to repeat the steps till the level variable value is less than 5.

—  In the loop, we present the user with the set of letters by using a for loop to and using which the user has to guess 3 words.

—  Next, inside this while loop, we have declared an integer variable wordCount to control the number of words the user can create at 
    each level, we have initialized it to 0.

—  We have declared a boolean variable match as a flag to control whether the word that the user has given as input matches with the one 
    declared in the array, we have initialized it to false.

—  We have declared two String variables, the first variable word will get the user input and the variable oldWord will maintain the 
    previous word so that if the user enters the same word again it will not be considered.

—  Inside the outer while loop we have created an inner while loop to take the word from the user, here the variable wordCount is used 
    in the condition to control that the user enters three correct words at each level.

—  Within this while loop first assign the value false to match variable assuming that the user will make the wrong guess and then we 
    take the user input and then compare it with the oldWord value.

—  If the current input does not match with the oldWord variable value, then we compare the user input with each word in the words array.

—  If the match is found in the words array, then the wordCount variable value will be incremented by 1, the value of the match variable 
    will be set to true, this current word will be set as value for oldWord variable and also score value will be incremented by 1.

—  After all the assignments, we break out of the for loop used to compare.

—  Lastly, in the while loop we check the value of the match variable, and if it is false we display the message to the user 'Wrong 
    Guess and will decrement the value of the lives variable by 1 and continue the loop for the next input.

—  Within the loop we also check if the value of lives variable has become equal to zero. If yes then we will display the message 'Game 
    Over!!! Better Luck Next Time!!! . We will also display the final score of the user and will break out of this inner while loop.

—  Within the outer while loop, but after the inner while loop, i.e. after the end of the level, we will reassign the variables 
    wordCount, match and oldWord to 0, false and '' respectively.

—  Within the outer while loop, next we will check if the value of the lives variable is equal to the zero. If yes we will break the 
    outer while loop and the game will stop.

—  Lastly, inside the outer while loop, if this while loop is running for the last level. If yes then we will display the message 
    "Thanks for playing the game!!!" to the user. We will also display the final score of the user.

—  If this is not the last level then we ask the user a question by displaying the message "Do you want to continue to the next level? 
    (y/n)".

—  If the user enters 'y', we just increment the value of the level variable by 1 and continue to the next level.

—  If the user enters 'n', or any other character, we stop the game. We will display the message "Thanks for playing the game!!!" to the 
    user. We will also display the final score of the user.

1. All that's left is to display the scores and have you create some more minigames!

2. To display the score you need to go back to Screen1's blocks. 

3. Down in the `call [File1].AppendToFile` block take the `get [global score]` block off and replace it witha  **Text** `join` block.

4. Hit the ![](/assets/symbol.png) symbol and drag another `string` over. 

5. put the `get [global score]` back in the center and two empty **Text** blocks on the top and bottom.

6. The top **Text** block is to add a space between the players name and the score. I used ": " as a spacer. Put "\n" in the last **Text** block. "\n" is how programmers tell the computer to hit "Enter" when it is displaying text. Here's what the blocks look like now: 

    ![](/assets/fixedappendscore.png)
    
7. Back on the home screen blocks, add a `when [HomeScreen].Initialize` block. From **File1** drag the `call [file1].ReadFrom` block and put a **Text** block on that says "player".

8. Great! You've read the text. Now you need to display it. Drag the `when [File1].GotText` block onto the screen from the **File1**. From **Label4** drag the `set [label4].[text] to` block into the previous block and put `get [text]` on the end.

9. Amazing! Your game is ready to go! 
1. You created all the parts for this app to work! Let's use these parts to make the app fun.

2. The screen that App Inventor always opens first is **Screen1**, but the player expects to see the home screen. So to open the home screen when the app starts you can use these blocks:

   ![](/assets/screen1initialize.png)

   * Note: This might be named something different if you chose another name for your home screen.

3. To control the app, all this screen needs to do is check what screen just closed. So, Drag the `when [Screen1].OtherScreenClosed` block from **Screen1** onto the **Viewer**.

4. When a minigame closes it results in a value. You can get this value inside the `when [Screen].OtherScreenClosed` block. 

5. To keep track of the player's score, you can use the `initialize global [name] to` block (in **Variables**). Change "name" to "score" so it's easy to remember. Drag the `[0]` block from math onto the `initialize global [score] to` block. Here's what it should look like:

   ![](/assets/otherscreenclose.png)

6. Drag the `if then` block with this symbol ![](/assets/symbol.png) into the `initialize local [score] to` block. click the symbol and drag two `else if` blocks over so it looks like this:

   ![](/assets/else if.png)

7. The first thing to check is whether a minigame closed or it was the home screen that closed. Using the `[] = []` block from **Logic**. Check if the `result` equals the text "HomeScreen" 

   * Note: Remember the home screen ends with the result "HomeScreen".

8. For the `then` part you want to play a minigame, because the only way the player got to **Screen1** from the home screen was pressing the play button. Remember the procedure you created? openMinigame? You can use that now. In **Procedures** there will now be a `call [openMinigame]` block, use that! You also need to use the `set [global score] to1 block to 0, or else so the game resets a new players score! Make sure everything in your blocks looks right:

   ![](/assets/homescreenclose.png)

9. The two `else if`'s will check if the player won the last game or not. Remember when a minigame closes it results in the **Text** "won" or "lost". If they won, the app should add 1 to the player's score and open another minigame. You can use the `[] + []` block from **Math** and the score variable to add 1.

   ![](/assets/won.png)

10. If they lost, it saves their score to the file and opens the home screen. To add the score to the player file use the `call File1.AppendToFile` block (from **File1**). After the score is saved, open the home screen. Here's how the blocks look:

   ![](/assets/lost.png)

11. You can try the app out now, but the score won't be working... You'll fix that on the next card!




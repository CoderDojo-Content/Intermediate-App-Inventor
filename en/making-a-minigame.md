1. This app is all about minigames! The first minigame were going to make will test your reflexes! Make a new screen named "Minigame1".

2. Add a label to your screen and make the text say "Touch the ball" \(this is so the player knows what to do!\). Under **\(Palette &gt; Drawing and Animation\)** add a canvas and then add a ball anywhere on the canvas.

3. The last thing you need is a clock **\(Palette &gt; Sensors\)**. Click the clock in **Components**. Uncheck **Timer Enabled** and set **TimerInterval** to 3000.

  ![](/assets/clockproperties.png)

4. Switch over to the **Blocks** view. You're going use the clock to see if the player can touch the ball fast enough! Here's the blocks:

   ![](/assets/startclock.png)

   The `set [Clock1].[TimerEnabled] to` is in the **Clock1** blocks. the `[true]` block is in ** Logic**.

5. Now the minigame just needs to decide if the player won or lost. If the player touches the ball before the clock timer goes off they win! If they don't...they lose.

6. Use the `when [Ball1].Touched` block and inside that we want to stop the timer. Use the same blocks as before but switch "true" to "false". Then add a `close screen with value result` block with the **Text** "won".

   From the **Clock1** blocks get the `when [Clock1].Timer` and put the `close screen with value result` and the **Text** "lost".

   Your blocks should look something like this:  
   ![](/assets/minigamewinorlose1.png)




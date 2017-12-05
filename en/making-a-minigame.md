1. This app is all about minigames! The first minigame were going to make will test your reflexes! Make a new screen named "Minigame1".

2. Add a label to your screen and make the text says "Record a sound quickly" \(this is so the player knows what to do!\). Also add two buttons ("Record" and "Stop"). Uncheck the **visible** option for the stop button. Under **\(Palette > Media\)** add a **SoundRecorder** to the screen.

3. The last thing you need is a clock **\(Palette > Sensors\)**. Click the clock in **Components**. Uncheck **Timer Enabled** and set **TimerInterval** to 3000.

  ![](en/assets/clockproperties.png)

4. Switch over to the **Blocks** view. You're going use the clock to see if the player can record a sound fast enough! Here's the blocks:

   ![](en/assets/startclock.png)

   The `set [Clock1].[TimerEnabled] to` is in the **Clock1** blocks. the `[true]` block is in ** Logic**.

5. Now the minigame just needs to decide if the player won or lost. If the player records a sound before the clock timer goes off they win! If they don't...they lose.

6. Drag two `when [button].Click` blocks onto the screen. 

7. Then from the **SoundRecorder** put the `call SoundRecorder1.Start` in your "record" button. To make the stop button visible, use the `set [Button2].[Visible] to` from **Button2**.

8. For the "Stop" button add the `set [Clock1].TimerEnabled to` with the `[true]` block from **Logic**. `call SoundRecorder1.Stop`. Then all you need to do is use the `close screen with value result` block and use the **Text** "won".

9. From the **Clock1** blocks get the `when [Clock1].Timer` and put the `close screen with value result` and the **Text** "lost".

   Your blocks should look something like this:  
   
   ![](en/assets/soundrecordingminigame.png)




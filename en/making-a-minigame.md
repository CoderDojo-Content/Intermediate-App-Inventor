1. This app is all about minigames! The first minigame were going to make will test your reflexes! Make a new screen named "Minigame1".

2. Add a label to your screen and make the text say "Record a sound quickly" \(this is so the player knows what to do!\). Also add two buttons ("Record" and "Stop"). Uncheck the **visible** property for the stop button. Under **\(Palette > Media\)** add a **SoundRecorder** to the screen.

3. The last thing you need is a clock **\(Palette > Sensors\)**. Click the clock in **Components**. Set **TimerInterval** to 3000 in its **Properties**.

  ![](/assets/clockproperties.png)

4. Switch over to the **Blocks** view. You're going use the clock to see if the player can record a sound fast enough!

5. Now the minigame just needs to decide if the player won or lost. If the player records a sound before the clock timer goes off they win! If they don't...they lose.

6. Drag two `when [button].Click` blocks onto the screen.

7. Then from the **SoundRecorder** put the `call SoundRecorder1.Start` in your "record" button. To make the stop button visible, get the `set [Button2].[Visible] to` from **Button2** and attach it to a `True` block.

8. For the "Stop" button add the `set [Clock1].TimerEnabled to` with the `[false]` block from **Logic**. Use the `call [SoundRecorder1].Stop` (from **SoundRecorder1**) to stop the recording. Then all you need to do is use the `close screen with value result` block and use the **Text** "won".

9. From the **Clock1** blocks get the `when [Clock1].Timer` and put the `close screen with value result` and the **Text** "lost". To make sure the recordings stopped add the `call [SoundRecorder1].Stop` here too.

   Your blocks should look something like this:  

   ![](/assets/soundrecordingminigame.png)

10. If you want to try the minigame out now just add two `set [Label1].Text to` blocks before you close the screen. Add the **Text** "won" and the **Text** "lost" to the appropriate block. Here's what mine looks like:

  ![](/assets/testingminigame.png)

11. Brilliant! If you want to try the game out now you need to do one more thing. Go back to the **HomeScreen** and right click on the `close screen with value result` block. The click **Add comment**. Programmers often use this to make the computer ignore a bit of code.

   ![](/assets/addingAComment.png)

12. Instead we want to show your new minigame. Just add the `open another screen screenName` block and attach it to a `""` block with "minigame1" in it.

13. Great, try out your game now! The text at the top of the screen will change and tell you if you won or lost!

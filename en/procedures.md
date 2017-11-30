1. The best way to make this app is by using a screen to control everything. Open Screen1 (with the button on the top left). 

2. The components this screen needs are a file **Storage** and a TinyDB **Storage**. Add these to the screen.

3. Now, open up the blocks page for the screen. You're going to make your first procedure! A procedure is a bit of code that you can use with its "call" block. Most of the time coders will use these blocks so that they don't need to create the same code twice (or even more).

4. Click **Procedures** on the left of the screen and drag over the `to [procedure] do` block. You're going to open you minigames with this procedure, so to help remember what this procedure does you can rename it "openMinigame".
 
5. Since you're opening a screen, drag the **Control** block `open another screen screenName` into the **Procedure** block.

6. This procedure is going to work for multiple minigames. (Don't worry about only having one minigame. I'll show you how to make some more later). For now you an drag the `initalize global [name] to` block from **Variables** on to the **Viewer**. Change "name" to "numberOfGames" (this helps you remeber what the variable is for). Just drag the `[0]` block onto end of the variable and change 0 to 1 and this variable is ready to go!

 * It should look like this:
 ![](/assets/globalVariable.png)
 
7. The last step is choosing a screen to open! Remember what the name of the screen for the first minigame was? Minigame1. To make things more interesting lets randomly  
 
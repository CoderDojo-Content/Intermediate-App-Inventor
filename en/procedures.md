1. The best way to make this app is by using a screen to control everything. Open Screen1 \(with the button on the top left\).

2. This screen also needs the **File** component. Add one to the screen.

3. Now, open up the blocks page for the screen. You're going to make your first procedure! A procedure is a bit of code that you can use with its "call" block. Most of the time coders will use these blocks so that they don't need to create the same code twice \(or even more\). These are the blocks we will use:

   ![](/assets/procedures.png)

4. Click **Procedures** on the left of the screen and drag over the `to [procedure]` block. You're going to open you minigames with this procedure, so to help remember what this procedure does you can rename it "openMinigame".

5. Since you're opening a screen, drag the **Control** block `open another screen screenName` into the **Procedure** block.

6. This procedure is going to work for your multiple minigames. Drag the `initalize global [name]` block from **Variables** on to the **Viewer**. Change "name" to "numberOfGames" \(this helps you remember what the variable is for\). Just drag the `[0]` block onto end of the variable and change 0 to 2 \(this is the number of minigames you have so far\) and this variable is ready to go!

   * It should look like this:

     ![](/assets/numberOfGames.png)

7. The last step is choosing a screen to open! Remember what the name of the screen for the first two minigames were? Minigame1 and Minigame2. This allows you to easily choose a random screen. Randomness will make your app feel different everytime.

8. To choose a random minigame you need 4 blocks: `join` block from **Text** \(puts two texts together\), `random integer from [1] to [100]` block from **Math**, `get[]`from **Variables**, and a **Text** block that has "Minigame" in it. Put them together so they look like this:

   ![](/assets/procedure.png)

   * Note: this is also how all these steps put together should look.

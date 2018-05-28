1. Awesome, you have your first minigame! Making more minigames will keep your app interesting everytime someone plays it. So let's make a minigame that uses a **List**.

2. A **List** is a bunch of items (variables) you store together. You can think about it like a grocery list. The list has oranges, apples, and grapes. They are items, but they're all on the same list because they're fruits.

3. Add a screen called "Minigame2". You can use the **ListPicker** (**Palette > User Interface**) to have the user pick an item in a list. Add one to the screen.

4. Switch over to the **Blocks Viewer**. Add the `initialize global [name] to` block and change "name" to something more descriptive: "wordsList".

5. There is a `make a list` block under **Lists**, drag that onto the **viewer**. Hit the ![](/assets/symbol.png) symbol and add some more items to the list. (I have 4 items, but you can use a different amount)

6. Now use `""` blocks to fill the empty spots on the list. Write words in them. I used different types of pets! This is what mine looks like:

    ![](/assets/petList.png)

7. In the **ListPicker** blocks there is a `when [ListPicker1].BeforePicking` block and a `set [ListPicker1].[Elements] to` block. Put these blocks together. Now all you need to do is put the `get []` **Variables** block on and then the **ListPicker** is ready! It will look like this:

    ![#](/assets/beforePicking.png)

8. When the player picks a word, you need to see if they chose the right word. You want to use the `when [ListPicker1].AfterPicking` block to check what word the player chose! Drag it onto the screen.

9. Choose a word from your list (I chose bird from mine). Back in the Designer, add a label and have it say "Choose" + whatever word you want them to choose!

10. Since were checking *if* the player chose the right word, you can use an if statement. Click the ![](/assets/symbol.png) symbol and add an else to the if.

11. For the if, use the `[] = []` block from **Logic**, a **Text** block, and the `[ListPicker].[Selection]` (the players choice) block from **ListPicker**. If the player's choice is right then close the screen with "won" else close with "lost".

12. Here's what it should look like:

    ![](/assets/afterPicking.png)

13. To check if it's working you can do what you did in the last minigame. Add two `set [label1].[Text] to` bocks and attach them with either `[won]` or `[lost]`.

14. You'll also need to change which screen opens when you click the "Play" button. Try and figure out how to do it! Then you can play your new minigame.

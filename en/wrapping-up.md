1. You have all the control of 
your app working! Now it is super easy for you to add your own minigames. I'll walk you thorough adding one more game then you can try and make your own minigames! 
 
2. Create a "Minigame3" screen (for your fourth game change 3 to 4 and so on with every game you make).

3. The game will see if the player can guess how much is being added to a number. So you need to add 2 labels, a TextBox, and a button in the **Designer**. here's how mine looks:

 ![](/assets/lastminigame.png)

4. Swap over to the blocks viewer. Using a for each loop will make this game easier to code. A for each loop repeats the same code until its stopped. This is useful for us lazy programmers! 

5. Use a `when Minigame3.Initialize` block and put an `initialize local [name] to` block in it. Set the variables name to "numbersText".

6. Now add a `for each [number] from` block (it's in **Control**). The for block has 3 pieces. The first is what number to start at, the second is how high the loop will count before it stops, and the last is how much the loop goes up by every time (this is what your player needs to guess). Set the first block to 0, the next to 10, and the last to 2:

  ![](/assets/forloop.png)

7. Now inside the for loop you can actually do something cool! Use the `set [numbersText] to` block. You're going to set it to the previous numbersText + a space (" ") + the number (this comes from the for loop. 

8. Now you just got to set the label's text to the `get numbersText` block and everything should look like this:

 ![](/assets/finishedforloop.png)

9. You've done this step before, see if you can understand why you need to add these code blocks:


10. Just go back to Screen1 and make sure the `initialize [numberOfGames] to` block is set to the number of games you have (3 right now)! 

11. Do you see how easy it was to add a game? Try some of these ideas for games:
  
  * First try to think of a game yourself (those are always more fun).
  
  * Change up the list minigame. Try to make the game select a random item in the list, tell the layer to click it, and see if the player picked the right choice.
  
  * Play around with other **Media** options. You can have the player take a picture of themselves with the camera blocks.
  
  * See if the player can tap a button 5 times in a second.
  
  * You can always make up your own games. Don't be afraid to get silly and try putting some blocks together!



  
1. You can make a **Home Screen**. This can also be called the start or main screen. You can create your own home screen by add a new screen and naming what you like (I chose "HomeScreen").

2. Lets put some of your skills from the first tutorial to the test! Try adding three labels and two buttons to the screen. It would be neat if the first label was the name of your app!

    Note: I like my home screen to be centered, so every thing isn't on the left. You can do this too by clicking on your screen in the **Components** menu then under **Properties** switch **AlignHorizontal** to *Center: 3*.
    
    ![](/assets/center.PNG)
    
3. Lets do something new now! You can get user input with the  **TextBox** in **(Palette > User Interface)**. Drag one onto your screen!

4. You are going to have your player play a bunch of mini games, so you can keep track of how many they win. Add a TinyDB to your screen. Also under **(Palette > Storage)** drag a **File** onto the screen. To display the score you will use a **ListView** this is under **(Palette > User Interface)**. Drag one onto your screen!

5. Make some final touches to your game so it looks like this:

    ![](/assets/homescreen.png)
    
    Note: You can make your layout look however you want, this is just what I did!
    
6. Time to add some code to your home screen. Open the blocks editor on the top right of the browser window.

7. You'll make the scoring display later, don't worry about it right now. Get the **When [button] .Click** code block and put two **call [TinyDB] .StoreValue** code blocks inside of it.

 8. Add a blank **Text** block to the tag of the first **.StoreValue** block. Put "name" in the **Text** block. To get user input, the block you need will be under the **TextBox** and looks like this: ![](/assets/text.png) 
 That's it! You just stored the users input in a database.
 
9.To finish up the block 
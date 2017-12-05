1. You can make a **Home Screen**. This can also be called the start or main screen. You can create your own home screen by add a new screen and naming what you like \(I chose "HomeScreen"\).

2. Lets put some of your skills from the first tutorial to the test! Try adding three labels and a button to the screen. It would be neat if the first label was the name of your app!

   Note: I like my home screen to be centered, so everything isn't on the left. You can do this too by clicking on your screen in the **Components** menu then under **Properties** switch **AlignHorizontal** to _Center: 3_.

   ![](/assets/center.PNG)

3. Lets do something new now! You can get user input with the  **TextBox** in **\(Palette &gt; User Interface\)**. Drag one onto your screen!

4. You are going to have your player play a bunch of mini games, so you can keep track of how many games they win. Under **\(Palette &gt; Storage\)** drag a **File** onto the screen. The app will use this to keep track of the players score!

5. Make some final touches to your game's home screen. Here's what mine looks like:

   ![](/assets/homescreen.png)

   Note: You can make your layout look however you want, this is just what I did!

6. Time to add some code to your home screen. Open the blocks editor on the top right of the browser window.

7. You'll make the scoring display later, don't worry about it right now. Get the `when [button] .Click` code block and put a `call [file1].AppendToFile` block in it from **File1**.

8. Add a blank **Text** block to the fileName spot. Put "player" in the **Text** block. This file will keep track of information about the player. To get user input, the block you need will be under the **TextBox** and looks like this:

   ![](/assets/text.png)

   Put it in the text spot:

   ![](/assets/button1click.png)

      That's it! You just stored the users input in the "player" file.

1. To finish up the block use the `call [TextBox].HideKeyboard` block from **TextBox1** and from **Control** the `close screen with value result` block. put a text block in with "HomeScreen". Like this:

   ![](/assets/finishedhomescreen.png)




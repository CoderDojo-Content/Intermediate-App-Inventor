1. A **Home Screen** can display information to your players. This can also be called the start or main screen. You can create your own home screen by adding a new screen and naming it what you like \(I chose "HomeScreen"\).

2. Lets put some of your skills from the first tutorial to the test! Try adding two labels and a button to the screen. It would be neat if the first label was the name of your app!

   Note: I like my home screen to be centered, so everything isn't on the left. You can do this too by clicking on your screen in the **Components** menu then under **Properties** switch **AlignHorizontal** to _Center: 3_.

   ![](/assets/center.PNG)

3. Lets do something new now! You can get user input with the  **TextBox** in **\(Palette &gt; User Interface\)**. Drag one onto your screen!

4. You are going to have your player play a bunch of mini games, so you need to keep track of how many games they win. Under **\(Palette &gt; Storage\)** drag a **File** onto the screen. The app will use this to keep track of the player's score!

5. Make some final touches to your game's home screen. Here's what mine looks like:

   ![](/assets/homescreen.png)

   Note: You can make your layout look however you want, this is just what I did!

6. Time to add some code to your home screen. Open the blocks editor on the top right of the browser window.

7. Get the `when [button] .Click` code block and put a `call [file1].AppendToFile` block in it from **File1**.

8. Add a blank **Text** block to the fileName spot. Put "player" in the **Text** block. This file will keep track of information about the player. To get the user's input, the block you need will be under the **TextBox** and looks like this:

   ![](/assets/text.png)

   Put it in the text spot:

   ![](/assets/button1click.png)

      That's it! You just stored the user's input in the "player" file.

9. To finish up the block use the `call [TextBox].HideKeyboard` block from **TextBox1** and from **Control** the `close screen with value result` block. Attach a text block with "HomeScreen". Like this:

   ![](/assets/finishedhomescreen.png)

10. Great! One last thing, you need to let the player see your homescreen. Currently the screen that App Inventor displays first is Screen1. To open the home screen when the app starts you can use these blocks(In the Screen1 blocks section):

   ![](/assets/screen1initialize.png)

10. If you run your app on the emulator or your android device you can see what the home screen will look like.

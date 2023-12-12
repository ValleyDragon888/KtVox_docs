# Game Loop

A game loop is the backbone of your game. It loops
around, and every frame re-draws the screen.

But first we need to initialise the window:
 ```
 fun main() {
     w = Window(20, 20)
 }
 ```

This creates the window, with a width and height of 20.
It'll just be blank at the moment though.

Next, every frame, the game loop needs to do 3 things:
1. clear the screen
2. re-draw the scene
3. and then update the screen (or, terminal)
4. Finally, wait for a bit.

Here is some code to do this:

 ```
 fun main() {
     w = Window(20, 20)
     while(true) {
         w.clear()
         // Code to draw stuff
         w.printScreen()
         Thread.sleep(100)
     }
 }
 ```
In this snippet, the `while(true)` repeats indefinitely,
`w.clear()` clears the screen, and `w.printScreen()` updates the terminal.

Now, lets do some interesting stuff.


# Showing Things on the Screen

This time, we will actually show things on the screen. Promise.

So, let's start with the same code as last time:

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

 What we need to do now, is replace `// Code to draw stuff`, with code to draw stuff.

 Replace it with

 ```w.drawBoxOutline(
        topLeft = XYPosition(0, 0)
        botomRight = XYPosition(5, 5)
 )```
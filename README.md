# Pong
A 1-player Pong game versus a low level computer. 

  This Pong game was programmed using the Turbo Macro Pro c64 assembler within the Versatile Commodore Emulator (VICE). The decision to use these tools were made on the account of a class I partook in focusing on retro computing, particularly during the "8-bit/6502 era" and on the Commodore. This program can be broken down into a few sections. 
  
  First is the graphical design asepct. There were many decisions to be made on how I wanted the game to look. Many aspects, such as the background, border, sprites(ball paddles), and text, required many tweaks and runs to the program to determine if all these pieces meshed well and looked good. As mentioned before, I designed and implemented 3 total sprites, the ball and two paddles. This would allow the paddles and ball to interact with each other, as well as move in a desired manner in order to create the game of pong. 
  
  The second large component of this program is the overall gameplay choices. This would include how fast the ball can move, if it can speed up over the course of the round, how fast the paddles are able to move, how strong the computer is, etc. All of these variables for the gameplay were dependent on the ball and paddle sprites, making them perhaps the most important piece of this entire program. In the future, I wish to make some adjustments to the size and overall smoothness of these sprites. 

  The last major section of this program is allowing for player input. I am still working on connecting a SNES controller to a computer via USB to allow a player to control one of the paddles. For now, the paddles are both controlled by low level computers that will start going towards the ball sprites Y-coordinate only when the ball gets so close to each paddle. 


  Due to wanting to modify the program to work, the way I intend it to, on a computer (without the need for a real-live Commodore), there are a couple bugs I will need to iron out. The main issue being the left paddle wanting to bug out occassionly. I should also mention that due to wanting to make this program work on a computer, I do not have player input implemented yet. For now, both paddles should perfectly mimic the balls movement (aside from the bug previously mentioned). Additionally, after a point is scored the game should reset the board and start another round. However, the game won't continue without player input, which is not yet implemented. I wish to implement player input via a USB SNES controller or keyboard in the future.


HOW TO RUN:
Before anything, you must download the pong.d64 file attached, this will contain all the needed files to run this program using the two tools listed below.

1. Download and install the Versatile Commodore Emulator (VICE) onto your computer. ( https://vice-emu.sourceforge.io/index.html#download )
2. Download and install the Turbo Macro Pro c64 assembler (TMP) onto your computer. ( https://style64.org/release/turbo-macro-pro-sep06-style )
3. Open VICE by going clicking on the VICE folder then open "GTK3VICE-3.7-win64" -> "bin" -> "x64sc".
4. Once VICE is loaded, click "file" on the top left and then click "attach disk image" -> "drive 8" then find and attach the TMPx download.
5. Once attached type load"$",8, press enter and then type "list" and press enter.
6. A variety of files will be listed, go to the one that says   73   "TMP           v1.s/S." prg. Using the arrow keys.
7. To load this file and open TMP, you must type "load" in place of the "73" and then delete the "prg" at the end, and replace it with ",8,1".
8. Run TMPx by typing "sys 32768" and press enter.
9. Now detach drive 8 and attach Pong onto drive 8.
11. Then press shift + tilda (key to the left of 1/!) and then press L (load). Type "pong.prg" and press enter.
12. The Pong program should be displayed at this point. Press shift+tilda 1 to exit the editor, then type "sys 4096" and press enter to run the program.
    

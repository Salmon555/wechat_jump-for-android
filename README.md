# wechat_jump-for-android
A python program for automatically playing a wechat game called Jump( Sorry for the Chinese annotation in the code)

The rules for this game is simply: You control a small cube to jump from a platform to another, the longer time you touch
the screen, the longer distance you will jump. You have to land on the next platform otherwise you will fall and lose the game.
The more platforms you reach, the higher score you will get.

It uses the os library and a usb cable to connect the Andriod cell phone and the computer.
The computer send a command line using a ADB Shell to simulate one touch on the cell phone. You have to install the ADB Shell before you run this program.
Every time you download the screenshot of your cell phone, you make a calculation of the distance between you and the center of your next platform in the pixel level. 
The algorithm in finding the center of a platform is using the color difference between platform and background. Using RGB color pattern.
After lots of experiments you calculate the best ratio of touching time to target distance.

Then your computer will automatically do the trick for you. And you can show off to your friend for getting a unbeliveably high score in the leaderboard. XD

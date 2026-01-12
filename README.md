This is how to make the Mbot Mega connect to a PS5 controller, but still connected to the computer

1.Connect your PS5 controller to your pc by pressing the PlayStation button and the action button until it starts to blink, then connect it to Bluetooth
2.Then go to python.org and download Python 3.x
3.When the download screen pops up go to the bottom and press add to path, then press install now
4.Now go to https://www.arduino.cc/en/software/ and scroll down until you see legacy IDE 1.8.19 and download it
5.Now copy adn paste "Arduino file." to ardrino ide
6.Now go to GitHub, write makeblock libay, and download the first one
7.Go back to Arduino IDE, go to sketch, and then to add.zip libary navigate to the file you just downloaded the library, and double-click on it.
8.Now go to comand line and type python --version. If it says 3.x or any number after you did everything correctly
9.Now type pip install pyserial inputs to download the library
10.then type pip install pygame
10.Now go and make a file in Documents and name it Mbot_ps5
11.Now, go to Notepad and copy th python code in here and paste it
12.Save it as the notepad and name it Mbot_bluetooth.py, write .py or it will not work.
13.Go back to Arduino IDE and upload it to the MBOT Mega
14.It does not work. Go to tools and put the board as mega 2560 and the processor atmega 2560 16 
15.go and check the notepad where it says Arduino = serial.Serial('COM4', 9600) change the (COM 4 ) to whatever you have on in toold in ardrino ide
16..Now go to comand line after uploading the Arduino code and type cd C:\Users\insert your name\OneDrive\Documents\megapiconroller by doing Ctrl Shift V make sure to put your naem of the computer or it will not work
17.If it was succsesull it should look like this: C:\Users\you name\OneDrive\Documents\Mbot_ps5>
18.Then type python Mbot_bluetooth.py to start
19.Now you can control you mbot mega with you ps5 controller

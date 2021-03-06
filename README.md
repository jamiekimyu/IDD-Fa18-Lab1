# IDD-Fa18-Lab1: Blink!

**A lab report by Jamie Yu**

## Part A. Set Up a Breadboard

![Breadboard Setup](https://github.com/jamiekimyu/IDD-Fa18-Lab1/blob/master/20180830_182631.jpg)


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**
The color stripes on the resistor are: red, red, black, black, and brown
 
**b. What do you have to do to light your LED?**
You have to setup the breadboard so the 5V are running across the right powerlines. Once the circuits are all setup, you connect the board to power from a laptop and then push the button. This closes the circuit and delivers power to the LED, lighting it up.

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**
You don't need to change any lines of code; simple upload the blink example code from the arduino website.

**b. What line(s) of code do you need to change to change the rate of blinking?**
I changed the number inisde the `delay(1000)` line to control the rate of blinking. 

**c. What circuit element would you want to add to protect the board and external LED?**
You would want to add a resistor. 
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**
You can no longer perceive the LED blinking at 14ms. You can prove that it is still blinking by recording it and slowing down the speed of the video. 

**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**

[Link to Code](https://github.com/jamiekimyu/IDD-Fa18-Lab1/blob/master/blink.ino)


### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[Link to Video, Pin 9](https://www.youtube.com/watch?v=OGSAxZq8ARE&pbjreload=10)


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**
I was able to get the LED to glow the whole turning range of the potentiometer. The potentiometer aska as a resistor with tunable resistance, thus with maximum resistance the LED glow was dim but with no resistance the glow was bright. 

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**
I uploaded and ran the example 'Fade' code. All I had to do was make sure that the pin specified in the code was the pin powering the LED on the circuitboard.

**b. What is analogWrite()? How is that different than digitalWrite()?**
analogWrite() lets you adjust the voltage with values between 0 - 255 while digitalWrite() only lets you toggle between HIGH and LOW values. 


## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

![Schematic](https://github.com/jamiekimyu/IDD-Fa18-Lab1/blob/master/20180903_185457.jpg)
**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**
I took apart a calculator, which is a computer that is able to perform limited functions. Once buttons that correspond to certain numbers are pressed, the numbers are converted to binary and processed through a microprocessor that I assumed was the black, bircular area in the middle of the chip. Once the function is calculated the data is outputted through the tape or LCD ribbon to the screen.  

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**
Information is conveyed from the user by the pressing of buttons on the calculator(0-9,+,-,=, etc.) which is processed into electrical signals and outputter as data through the LCD ribbon to the screen.

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**
The device is powered through a 3V battery that is taped to the back of the chip. 

**d. Is information stored in your device? Where? How?**
The numbers inputted by the user are converted to binary and stored in the microprocessor. The processor remembers the numbers inputted while the calculator is on. 

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**
I looked for either exposed pins or resistors as natural points to try to hijack and implant an LED. I couldn't find an exposed PIN but I could see a metal area that had 'R1' next to it. When I put the long leg of the LED against the resistor the light turned on. I could toggle the LED light on and off by pressing the ON/OFF buttons on the calculator. 

### 3. Build your light!

[Frankenlight](https://www.youtube.com/watch?v=gsHtOze10VQ&pbjreload=10)

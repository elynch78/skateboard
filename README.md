# skateboard

## Table of Contents
* [Table of Contents](#TableOfContents)
* [Blink Led](#Blink_Led_CircuitPython)
* [CircuitPython_Servo](#CircuitPython_Servo)
* [CircuitPython_Distance LED](#CircuitPython_Distance_LED)
* [Photointurrupter](#Photointurrupter)
* [CircuitPython LCD](#Circuitpython_LCD)
---

## Skateboard 
### Description & Code
I had to make code in Mu that would make the Metro Express change colors. [This website](https://www.w3schools.com/colors/colors_picker.asp) was a great source because it had all the codes for lots of different colors. 


```
import board
import neopixel
import time

dot = neopixel.NeoPixel(board.NEOPIXEL, 1)

while True:
    dot.brightness = (.1)
    print("Make it red!")
    dot.fill((255, 51, 0))
    time.sleep(.5)
    print("Make it dark blue!")
    dot.fill((0, 0, 102))
    time.sleep(.5)
    print("Make it fuscia!")
    dot.fill((204, 0, 102))
    time.sleep(.5)
    print("Make it yellow!")
    dot.fill((255, 255, 0))
    time.sleep(.5)
```


### Evidence

![Blink led](Images/gif-led.gif)

### Wiring

No wiring was needed, the Metro express had the neopixel.

### Reflection
The led was changing too fast in the beginning, so I made the time.sleep (.5) seconds long so you could see each color fully before it switched to the next. It was easy to add more colors once you got the first 2 running, you would just copy the above code format, and then change the color you have written and the numbers for the color calibration. 






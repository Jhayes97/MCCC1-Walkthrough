# Stellar Epic Snake - 300
This challenge was really awful. It expects you to use an obscure steganography tool from 2006. Nothing fun about it.
# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sne1.PNG "Stepic")

# Guide

Ok, let's download this image and get started.

The prompt seems weird. I'm guessing it's something to do with Python but no there are endless amounts of Python stego tools.

After a long time of searching endlessly, I stumble across `Stepic`. That seems to match with the theme of **Ste**llar E**pic** Snake.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sne2.PNG "Stepic")


Reading up on the documentation, it looks like the syntax we should use is `./stepic -d -i ikr.png -o flag.jpg`, let's download the program and test it.


 After running the code, it seems we get an additional image out of `ikr.png`!


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sne3.PNG "Stepic")


There's our flag, 

**flag{PHI1LOS0R4PT3R}**

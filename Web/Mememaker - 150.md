# Mememaker - 150
This challenge was a bit wonky, it's solvable but not entirely by the intended solution.


# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/mem1.PNG "Logo Title Text 1")


# Guide

Based on the prompt, I'm guessing we have to edit our cookie value somehow. Let's check out the site

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/mem2.PNG "Logo Title Text 1")

Incredible, the website is a time machine to 2009. Let's follow the *hilarious* photo's advice and check out the source.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/mem3.PNG "Logo Title Text 1")

It's running a couple of JS scripts, let's check out users.js


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/mem4.PNG "Logo Title Text 1")

That looks like our flag, obscured to hell and back. We could edit our `username` cookie to equal `premium`, but it seems to overwrite it every time we refresh the site. Let's just throw this code in the console.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/mem5.PNG "Logo Title Text 1")

Running the code in our browser's console, we get our flag.

**flag{born2true}**

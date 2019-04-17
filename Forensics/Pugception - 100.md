# Pugception - 100
This CTF has a recurring theme of telling us everything. Since MCC2017 was pretty hard I guess they wanted more people to solve challenges.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pug1.PNG "Pugception")


# Guide
Alright, without knowing any besides the prompt we know exactly what we're doing. This is almost becoming laborious.

Let's download the image and run the tool it tells us to.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pug2.PNG "Pugception")

We downloaded the image and ran the tool. Now what has it found tacked on to the end of the image?

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pug3.PNG "Pugception")

It's a `.wav` file, it's hard to communicate what it says, but it sounds like a text to speech tool reading us our flag. Googling for speech to text we can find a tool to help us render it into a flag format.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pug4.PNG "Pugception")

We upload our file and well, that output is a bit confusing.

Manipulating a bit, we get

**flag{s3cp00pn}**

What does that mean? No idea.

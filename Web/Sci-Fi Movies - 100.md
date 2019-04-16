# Sci-Fi Movies - 100.md
This challenge involved a bit of foreknowledge and a bit of perception. I enjoyed this challenge as I have seen a similar challenge on a hackthebox machine.


# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci1.PNG "Logo Title Text 1")


# Guide
Interesting prompt, I think I know what they're referencing. Let's check out the website.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci2.PNG "Logo Title Text 1")

Again with the robots refernce. I'm betting we want to look at the `/robots.txt`

# robots.txt

If you didn't know, if a website wants to prevent a webcrawler from indexing certain pages, they will list the pages the crawler should not visit in the robots.txt

This can lead to some interesting results being hidden in there. Let's check it out.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci3.PNG "Logo Title Text 1")

A disallowed page? Let's investigate.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci4.PNG "Logo Title Text 1")


This doesn't look too interesting, let's look at the image.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci5.PNG "Logo Title Text 1")

If you're perceptive, or you've seen this sort of deal on a vuln box before, you'll notice the URL.

Where does this lead?

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci6.PNG "Logo Title Text 1")

We're on the right path! Nothing here looks too interesting so let's view the page source

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/sci7.PNG "Logo Title Text 1")

Got it!

**flag{apparently_1nterst3114r_is_stellar}**


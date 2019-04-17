# President's FTP - 150
This challenge was the only one not solved with strings, so it is by default the best of the category.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pfp1.PNG "PresFTP")


# Guide
The prompt mentions uploads, so I'm betting we can find some files inside of that pcap.

We're going to use a tool called `NetworkMiner`, as it is much more effective at extracting file uploads.

Let's see what files we can find by opening the pcap in NetworkMiner.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pfp2.PNG "PresFTP")

It's got tons of files, Let's start by sorting through the images and hope we get lucky.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pfp3.PNG "PresFTP")

This image looks very out of place, so I instantly noticed it. It also contains our flag!

**flag{coming_2_a_theater_n34r_u}**


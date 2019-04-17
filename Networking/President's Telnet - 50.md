# President's Telnet - 50

This category should be called `strings` because we'll use it to solve 3/4 of the challenges.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pres1.PNG "Logo Title Text 1")

# Guide
The prompt references Telnet. If you didn't know, Telnet is like SSH, except everything is in plaintext. With a pcap of Telnet traffic, we can easily obtain the password, or flag in this case.

Let's download the pcap and run `strings prez.pcap | fgrep 'flag`

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/pres2.PNG "Logo Title Text 1")

There's our flag, 

**flag{i_am_the_prez_plaintext_is_enuff_4_me}**

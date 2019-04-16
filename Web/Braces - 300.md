# Braces - 300
This challenge was neat, you get to use a tool mostly reserved for vuln hubs in a CTF. Overall it depended on your previous exposure to a SQLi vulnerability.


# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/br1.PNG "Braces")


# Guide

His site was hacked? Let's look at his site then.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/br2.PNG "Braces")

Well, that link looks incredibly vulnerable. Let's see if we can throw an  ` OR '1'='1' ` statement into it. 


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/br3.PNG "Braces")


We've partly dumped it, but I bet there is more to it.

Let's use a tool called `sqlmap` to enumerate it all for us.

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/br4.PNG "Braces")

Plugging in our vulnerable URL with `--dump` at the end, we let sqlmap run.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/br5.PNG "Braces")

It succesfully dumps the database, and we find our flag in the notes table

** flag{reta1n3rs_hur7} **

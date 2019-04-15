# Knapsack  - 400
This challenge was maybe the most difficult to understand in concept, but very simple once put together.


# Prompt

![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp1.PNG "Knapsack")


# Guide

Starting out I had no idea what any of this meant, so the first step was google. 

![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp2.PNG "Knapsack")

Okay, it looks like we're dealing with a public and a private key. Doing some further research we stumble on the `Merkle-Hellman Knapsack Cryptosystem`

Let's scroll down to the decryption section.

![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp3.PNG "Knapsack")

It looks like our private key is w,q, and r. All of which we were (somewhat) generously given. How can we decode the message with this now? First let's read the rest of the wikipedia article.

![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp4.PNG "Knapsack")

Ok, so we're going to take the encrypted message (msg), multiple each integer by the modular inverse(modInv), and then return that number mod q (q).
Let's see that in a python script.


![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp5.PNG "Knapsack")

and the result:


![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp6.PNG "Knapsack")


Now with this array, it looks like we will use the super increasing sequence and assign 1's or 0's based on if the number is able to be successfully subtracted from it.

Think of this as a true or false.

So we have `[482, 252, 644, 1101, 1059, 553, 678, 553, 397, 644, 988, 1199, 369, 1199, 1016, 59, 59, 252, 914]`
and `[2, 9, 16, 43, 71, 156, 301, 619]`. Let's start with the first number 482.


![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp7.PNG "Knapsack")

So we get the binary number `01100110`, or `f`. That seems correct, because we expect the first 4 letters to be `flag`.
It's quick enough to do in your head, but in the interest of keeping things a lesson, let's show off a python script that FCC Cyber team member `Jakob Denlinger` made for this problem.

![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp8.PNG "Knapsack")


Using Jakob's script, we get our flag

![alt text]( https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/knp9.PNG "Knapsack")

**flag{n1njas_r_k00l}**


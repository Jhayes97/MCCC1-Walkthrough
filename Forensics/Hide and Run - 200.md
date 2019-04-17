# Hide and Run  - 200
Finally no more spoonfeeding. This seems to be a standard Stego challenge, and based on the title I know what it wants.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/hid1.PNG "Hide")

# Guide

Reading the title alone, I'm betting it wants us to use `steghide`, which is a standard tool you should know if you plan on doing CTFs regularly.

Let's download the `.wav` file. 

Listening to it, I hate this challenge. The song is awful. 

I don't blame them because I've made a few stego challenges myself that make competitors listen to terrible songs, this is really just karma.


Having listened to the audio, it sounds like the name of the alligator is `schnappi`, so let's use `steghide` to extract data from it using that password.


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/hid2.PNG "Hide")

using the password `schnappi`, we recovered the flag file from the `.wav`. We use `cat` to view the contents and get our flag 

**flag{fil3s_can_hide_and_run}**

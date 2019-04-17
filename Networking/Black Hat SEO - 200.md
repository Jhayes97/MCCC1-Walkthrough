# Black Hat SEO - 200
Do you know the `strings` tool? Good, you can solve this.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/seo1.PNG "SEO")


# Guide
The prompt says that we're searching for a password, so let's run `strings mean_people_seo.pcapng | grep pass`


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/seo2.PNG "SEO")

At the very end of the results, we get this 


![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/seo3.PNG "SEO")


`login=oklahomasweet%40mailinator.com&register=0&password=727%40Nne6c0%23n`

so it looks like the password is `727%40Nne6c0%23n`. The `%40` and `%23` looks a little funny though, and it won't accept `727%40Nne6c0%23n` as the flag.


I think it may be URL encoding.

Finding a guide online it looks like...

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/seo4.PNG "SEO")

and 

![alt text](https://github.com/Jhayes97/MCCC1-Walkthrough/blob/master/src/seo5.PNG "SEO")

So it should really be `727@Nne6c0#n`

We try and it accepts! there is our flag!

**727@Nne6c0#n**

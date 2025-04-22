**Title**: Gallery  
**Platform**: Hack The Box
**URL**: https://tryhackme.com/room/gallery666

Scan

![](screenshot/gallery1.png)

In 8080:

![](screenshot/gallery2.png)

We search some dirs but no nothing interesting:

![](screenshot/gallery3.png)

So in the login panel I caputured the request

![](screenshot/gallery4.png)

Unsafe response... 

![](screenshot/gallery5.png)

Now we are inside

We can see some interesting things

![](screenshot/gallery9.png)

We can upload an avatar, I try upload my reverse shell php

![](screenshot/gallery8.png)

Later of upload and update, we can get connection in our listener 

Now inside, we can see the gallery directory and: 

![](screenshot/gallery11.png)

So: 

![](screenshot/gallery10.png)

Here are the hash administrator:

![](screenshot/gallery12.png)

Later of trying decrypt this hash. i didn't but I found this backup of the user mike:

![](screenshot/gallery13.png)

Interesting.. but this passwords not work. Anyway, the password are in the .bash_history

![](screenshot/gallery13-1.png)

Now we are the user Mike and we can get the user.txt

![](screenshot/gallery14.png)

Now we try be root, so run the command: sudo -l and detect a very strange .sh

![](screenshot/gallery15.png)

we can run /bin/nano like sudo 

![](screenshot/gallery16.png)

![](screenshot/gallery17.png)

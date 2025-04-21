**Title**: Gallery  
**Platform**: Hack The Box
**URL**: https://tryhackme.com/room/gallery666

Scan

![t](img/gallery1.png)

In 8080:

![](img/gallery2.png)

We search some dirs but no nothing interesting:

![](img/gallery3.png)

So in the login panel I caputured the request

![](img/gallery4.png)

Unsafe response... 

![](img/gallery5.png)

Now we are inside

We can see some interesting things

![](img/gallery9.png)

We can upload an avatar, I try upload my reverse shell php

![](img/gallery8.png)

Later of upload and update, we can get connection in our listener 

Now inside, we can see the gallery directory and: 

![](img/gallery11.png)

So: 

![](img/gallery10.png)

Here are the hash administrator:

![](img/gallery12.png)

Later of trying decrypt this hash. i didn't but I found this backup of the user mike:

![](img/gallery13.png)

Interesting.. but this passwords not work. Anyway, the password are in the .bash_history

![](img/gallery13-1.png)

Now we are the user Mike and we can get the user.txt

![](img/gallery14.png)

Now we try be root, so run the command: sudo -l and detect a very strange .sh

![](img/gallery15.png)

we can run /bin/nano like sudo 

![](img/gallery16.png)

![](img/gallery17.png)

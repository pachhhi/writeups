**Title**: Gallery  
**Platform**: Hack The Box
**URL**: https://tryhackme.com/room/gallery666

Scan

![[gallery1.png]]

In 8080:

![[gallery2.png]]

We search some dirs but no nothing interesting:

![[gallery3.png]]

So in the login panel I caputured the request

![[gallery4 2.png]]

Unsafe response... 

![[gallery5.png]]

Now we are inside

We can see some interesting things

![[gallery9.png]]

We can upload an avatar, I try upload my reverse shell php

![[gallery8.png]]

Later of upload and update, we can get connection in our listener 

Now inside, we can see the gallery directory and: 

![[gallery11.png]]

So: 

![[gallery10 1.png]]

Here are the hash administrator:

![[gallery12.png]]

Later of trying decrypt this hash. i didn't but I found this backup of the user mike:

![[gallery13.png]]

Interesting.. but this passwords not work. Anyway, the password are in the .bash_history

![[gallery13-1.png]]

Now we are the user Mike and we can get the user.txt

![[gallery14.png]]

Now we try be root, so run the command: sudo -l and detect a very strange .sh

![[gallery15 1.png]]

we can run /bin/nano like sudo 

![[gallery16.png]]

![[gallery17.png]]
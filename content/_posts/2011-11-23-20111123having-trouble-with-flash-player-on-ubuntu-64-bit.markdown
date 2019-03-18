---
author: whennessy0725@gmail.com
date: '2011-11-23 09:25:17'
draft: false
title: Having Trouble with Flash Player on Ubuntu 64-bit?
type: post
url: /simple-strategies/2011/11/23/having-trouble-with-flash-player-on-ubuntu-64-bit
---




As I wrote earlier, I'm building [a cool application using Twilio](http://billhennessy.com/s/why-twiliowhy-twilio?format=original), the best solution for voice and text app development on the market.




But there's a problem.




**I prefer developing in Ubuntu** for reasons only a developer who loves hyper-rapid releases can understand. Twilio provides a fantastic testing tool right on my dashboard page at [www.twilio.com](http://www.twilio.com).




This testing tool is a Flash object that calls my Twilio number, allowing me to experience what my users will experience.




The problem is that the Settings object for Flash Player 64-bit is unclickable in Ubuntu 11.10. The little bugger wouldn't let me Allow access to my microphone, which is pretty important for voice phone app.




**The good news: I found a workaround. **




I posted this workaround on [Twilio's forum](http://getsatisfaction.com/twilio/topics/twilio_client_not_working_from_ubuntu_11_10_firefox_chrome?utm_content=topic_link&utm_medium=email&utm_source=reply_notification). Rob, a Twilio Developer Evangelist, suggested I blog it, too. Apparently, I'm not the only person having trouble with the 64-bit Flash Player.




**The Workaround**




 
  * First, try to use the client at twilio.  Flash Player Settings dialog  will open, but it's not clickable. (**You must visit the Twilio site first to  get the URL into Flash Player's cache**.) 
  * Next, go to [http://www.macromedia.com/support/doc...](http://www.macromedia.com/support/documentation/en/flashplayer/help/settings_manager02.html)
  * Click on the Website Privacy Settings tab (3rd from right in Global Privacy Settings panel) 
  * look for the URL to your twilio dashboard. It begins with GUID, so pay  attention to the far right-hand side of the URL column. You'll be able  to see  only the first few chaacters of .twilio. (There may be more than  one entry in the list--repeat this process for each of them.) 
  * Click on the twilio url. 
  * Select Alway Allow from the radio group above 
  * Restart Firefox (or Chrome) 
  * Celebrate your remarkable achievement!!!! 



Here's a screen shot of the Adobe dialog just in case my narrative is unclear. 


[![](https://s3.amazonaws.com/satisfaction-production/s3_images/632859/Settings_Manager_-_Website_Privacy_Settings_panel_inline.png)
](https://s3.amazonaws.com/satisfaction-production/s3_images/632859/Settings_Manager_-_Website_Privacy_Settings_panel.png)




Finally, many thanks to Devin and Rob at Twilio. They jumped on my forum post immediately and stuck with me to the end.




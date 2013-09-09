messagingkata-baconjs
=====================
Some docs to help you get going:   
https://github.com/baconjs/bacon.js     
http://www.cheatography.com/proloser/cheat-sheets/bacon-js/   
https://github.com/baconjs/bacon.js/wiki/Diagrams   
http://nullzzz.blogspot.fi/2012/11/baconjs-tutorial-part-ii-get-started.html  


THE KATA
--------
This kata simulates a simple email system. A user will type in one or more email messages into the "To" input field and a message in the "Message" input field. Now this isn't just some boring old email system. No, this system is for the geek who likes to see what's sent over the wire. So your job is to display a simplistic SMPT message as the geek is typing, cause well that's just the kind of person they are. Not only does this geek want to see the SMPT they also want to see any mistakes in realtime as their typing. You forget an @ symbol in an address, show that error. 


STEPS
------
**One address, simple message:**  
to: joe@example.com  
message: Hi how's it going?
SEND Button is enabled
Network area shows:  
"connect smtp  
To: joe@example.com  
    
Hi there!  
  
disconnect  
"    

**Addresses need an '@' sign.**  
to: joenoatexample.com  
message: Hi how's it going?  
The incorrect address should be shown in the errors section.  With a note: Needs '@' sign  
The SEND Button is disabled.  
Network area shows:
"connect smtp  
To: joenoatexample.com  
    
Hi how's it going?  
  
disconnect  
"    

**Send to multiple addressess**  
to: sally@example.com joe@example.com  
message: Hi All.  
SEND Button is enabled
Network area shows:  
"connect smtp  
To: sally@example.com  
To: joe@example.com  
    
Hi All.  
  
disconnect  
"    


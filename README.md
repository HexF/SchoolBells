# SchoolBells

I created this as we had an old bell system that in order to change the times we had to remote into a server and because of where we had that running it was difficult to give multiple people access to it.
This uses the same usb relay:
![relay](relay.jpg =250x)
But has a web interface for scheduling the bells.
![relay](screenshot.png =250x)
![relay](screenshot2.png =250x)

Released as is where is for you to take as needed.
To run you need a usb relay, and a web server running PHP (can just be a crappy old machine)
You'll also need to add ring.php to your cron job list to run every minute like this:
`* * * * * cd /var/www/html && php ring.php`

**Our current setup:**
- Web server running on raspberry pi (although could run on any old - or new - computer you have lying around)
- Raspberry Pi has a static IP
- USB relay plugged into that

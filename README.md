#maxdeskstreamer

Max MSP tools to network stream a desktop capture and pipe through Syphon.

![alt text](https://raw.githubusercontent.com/ericrieper/maxdeskstreamer/master/misc/serverscreen.png "Server screenshot")

![alt text](https://raw.githubusercontent.com/ericrieper/maxdeskstreamer/master/misc/clientscreen.png "Client screenshot")

Uses `jit.net.send` and `jit.net.receive` to stream a `jit.desktop` matrix across local or remote network.

##Server Instructions
* Set your display Width and Height
	* Setting Width and Height lower than your display resolution will stream a cropped section of the display.
* Set IP and Port
* Set Frames Per Second for stream
	* `jit.net.receive` is very high bandwidth so using a slow FPS (2-8) is more reliable. Using a fast FPS causes both dropped frames and substantial latency.
* You can keep settings by clicking `Store Settings` and recall them with `Reset`. To save them for next time the patch is run, click `Store Settings` and then save the patch.

##Client Instructions
* Set incoming IP address or leave as "ALL"
* Set incoming Port Number
* Set `servername` for Syphon server- It will show up as "Max - [servername]' in your Syphon client.

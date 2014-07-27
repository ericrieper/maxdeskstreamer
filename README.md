maxdeskstreamer
===============

Max MSP tools to network stream a desktop capture.

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Uses `jit.net.send` and `jit.net.receive` to stream a `jit.desktop` matrix across local or remote network.

* Set your display Width and Height
	* Setting Width and Height lower than your display resolution will stream a cropped section of the display.
* Set IP and Port
* Set Frames Per Second for stream
	* `jit.net.receive` is very high bandwidth so using a slow FPS (2-8) is more reliable. Using a fast FPS causes both dropped frames and substantial latency.
* You can keep settings by clicking `Store Settings` and recall them with `Reset`. To save them for next time the patch is run, click `Store Settings` and then save the patch.

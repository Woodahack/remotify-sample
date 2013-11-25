Remotify sample app
===================

This is a sample app for the Remotify plugin available for the Corona SDK

>
> IMPORTANT, MUST READ
>
> The Remotify Plugin is Corona Simulator ONLY
>
> The Remotify Plugin NEEDS the Remotify app in order to work.
>
> The plugin ONLY works with the new graphics 2.0 engine
>

The app will be available through both the Apple App Store and the Google Play Store.

Once a user has the Remotify app installed on his/her device, all the user needs to do is insert the **require "plugin.remotify"**
line of code at the top of his/her project in main.lua. This line of code will activate the Remotify Plugin. No other functions need to be called.

If everything is working right, the Remotify plugin should show a blue bar which gives the user his/her IP address. This IP address should then be filled in at the Remotify App on an actual device. Then the connect button from the Remotify app should be pressed. The app will now show either a red(failure), blue(searching) or green(success) bar. If the red bar shows, the app is unable to connect to the simulator. Check if you have correctly required the Remotify plugin and that the simulator is showing a blue bar with a spinner.

Remotify enables users to control the simulator from a remote device. Therefore any sample app that makes use of Runtime touch, GPS, accelerometer, hardware keys or compass events should provided a test case for the Remotify Plugin.

All that needs to be done is:

* Have a working Remotify app and an internet connection
* Call the line 'require "plugin.remotify"' at the top of main.lua
* Make sure that the PC/MAC tested on is connected to the same local network as the device that runs the Remotify app


To test if everything is working the following should happen when you run the sample app:

1. After a few seconds it displays your IP address
2. On succesful connect, the white dot should begin to move due to the input of your device
3. With the current project turn on multitouch on the Remotify app by tapping the 'four squares' icon. Now when you tap the black overlay on your device white pointers should show on the simulator screen. Provided of course that a connection has been set up and the top bar of the Remotify app is blue
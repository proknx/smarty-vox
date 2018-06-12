# Using Smarty-Vox with realKNX v1 (Synology)

This guide explains how to integrate Smarty-Vox microphones and gateway with realKNX v1 (Synology EDS14). 
Please note that Smarty-Vox is fully integrated in realKNX v2 (revPI).

# Step 1: Find the Gateway
![Alt](http://proknx.com/en/news/2018/offline-voice-control-with-smarty-vox-privacy-guaranteed/planner-a4-1500x1500/ =300x300)

**Method 1:** Download and run the software “Packet Sender” from https://packetsender.com/,
Fill in the fields below with the following information:
ASCII: EMPERS_MQTT_ FIND, Address: 255.255.255.255, Port: 8888, choose
“UDP”, then press “Send”.
The IP and MAC address of ZNG100 will be displayed.
**Method 2:** Use Fing or similar app from your mobile device, look for vendor "AzureWave Technology"
In the address bar of browser, input the local IP of the Gateway. In the login
page, enter the default username and password : “admin”.

# Step 2: Pairing of devices 

 - Press the "+" symbol next to "Add or remove devices".
 - Press the "Add" button to add a device.
 - The status window shows the countdown message
 - Plug in the power of the microphone,  the blue light goes on when it is not yet paired with any gateway. 
- Turn the cover counter-clockwise to open it. 
- Press the pairing button on the device once to pair it with the gateway, the status window disappears after the device has been added, the blue light goes off.
- Then press the left “Device List”
- 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzMxNzYwMjk5LDU2ODgwNDg4MSwtMjI4MD
g2NDY5XX0=
-->
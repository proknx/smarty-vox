# Using Smarty-Vox with realKNX v1 (Synology)

This guide explains how to integrate Smarty-Vox microphones and gateway with realKNX v1 (Synology EDS14). 
Please note that Smarty-Vox is fully integrated in realKNX v2 (revPI).

# Step 1: Find the Gateway
![Smarty-Vox Gateway](http://proknx.com/en/news/2018/offline-voice-control-with-smarty-vox-privacy-guaranteed/planner-a4-1500x1500/ =300x300)

**Method 1:** 

Download and run the software “Packet Sender” from https://packetsender.com/,

Fill in the fields with the following information:
 - ASCII: EMPERS_MQTT_ FIND, 
 - Address: 255.255.255.255, 
 - Port: 8888, 
 - choose “UDP”, 
 - then press “Send”.

The IP and MAC address of ZNG100 will be displayed.

**Method 2:** 
Use Fing or similar app from your mobile device, look for vendor "AzureWave Technology"
In the address bar of browser, input the local IP of the Gateway.

In a browser, open the IP of the Gateway.
In the login page, enter 
 - username: "admin"
 - password : "admin"


# Step 2: Pairing of microphones 
![Smarty-Vox Microphone](https://proknx.com/wp-content/uploads/2018/06/zsr220new-1500x1000.png =300x200)

 - Press the "+" symbol next to "Add or remove devices".
 - Press the "Add" button to add a device.
 - The status window shows the countdown message
 - Plug in the power of the microphone,  the blue light goes on when it is not yet paired with any gateway. 
- Turn the cover counter-clockwise to open it. 
- Press the pairing button on the device once to pair it with the gateway, the status window disappears after the device has been added, the blue light goes off.
- Then press the left “Device List”
- repeat for all microphones


# Step 3: Add Node-RED action handler
1.  Open the  "Automation/Node-RED"  application from realKNX main menu. In the next step you will import the action handler flow in Node-RED.
2.  Open the  [Node-RED library](https://proknx.com/en/node-red-app/#node-red+s:smartyvox) . Under Download code,  select the an handler flow (e.g. '-   German v1 [offline-voice-smartyvox-de-v1.json](https://raw.githubusercontent.com/proknx/node-red-lib/master/offline-voice-smartyvox-de-v1.json)')
3.  Follow the instructions given in the Node-RED flow to import and customize the action handler. This video explains how to import  [Video Tutorial](https://screencast-o-matic.com/watch/cFVT63oOVU)

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0NDYyNTIwOTEsLTIyNDEyMjA2NCwtMz
g2OTY5NTc5LDMzMTc2MDI5OSw1Njg4MDQ4ODEsLTIyODA4NjQ2
OV19
-->
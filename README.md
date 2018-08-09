# Device location visualizer
This simple project is one example of how we can have a physical devise representing someone's location status
In this case I've used a Wemos D1 mini (esp8266) and a MicroOLED shield.
The Wemos connects through my WiFi network to an MQTT server and listens to value changes in the `{device_id}/location` topic.
If your current location tracking system already publishes changes to MQTT, then you can just change the topic and the states, otherwise it's very easy to plug this in your current system.

My case is pretty simple, I have 3 states `home`, `work` and `away`. To each state I've assigned a bitmap

Home
<img src="https://raw.githubusercontent.com/moopoint/device_location_visualizer/master/images/home.png" width="48">

Away
<img src="https://raw.githubusercontent.com/moopoint/device_location_visualizer/master/images/away.png" width="48">

Work
<img src="https://raw.githubusercontent.com/moopoint/device_location_visualizer/master/images/work.bmp" width="48">
